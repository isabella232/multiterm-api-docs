
# MTF Source

```xml
<Schema name="MTF" xmlns="urn:schemas-microsoft-com:xml-data" xmlns:dt="urn:schemas-microsoft-com:datatypes" xmlns:html="http://www.w3.org/TR/REC-html40">
       	<!-- DESCRIPTION -->       <!--
This schema describes the structure of a MultiTerm XML file. 
Copyright (C) 2000-2003 TRADOS Ireland Ltd., Dublin.

;; 
;; See http://msdn.microsoft.com/library/psdk/xmlsdk/xmls0390.htm for
;; the schema documentation.
;; 
 -->       <!-- HISTORY -->
       	<!--
;; 05-May-2000		Cornelis van der Laan	
;;    Removed <xref>, <termNote>, <admin>.
;;
;; 18-Jan-2000		Cornelis van der Laan	
;;    Removed TMX tags, because they apply to the exchange format TBX,
;;    not to the database-internal format we describe here.
;;    Added <xref> tag to <descrip> and <note> fields. 
;;    Added mandatory type attribute to the <language> tag.
;;
;;	10-04-2001		Milosavljevic Milosh	
;;
;;	    Added <xref> back to <descrip> tags.
;;	    Added <descripGrp> inside of <descripGrp> tags.
;;	    Remove <sourceGrp> and <noteGrp> tags. 
;;     Remove attribute lang from <descrip>
;;
;;17-07-2003			Michael Wetzel
;;
;;		     Bug fix: Changed element content of <descrip>element from
;; 	 "textOnly" to "mixed", since it can contain <xref> elements 
;;
;;
 -->      <!-- DEFAULT ATTRIBUTES -->      <!-- 
These attributes can in general be applied to all elements.
Note: 'type' is defined here, but for many elements, it will be overridden 
in favor of a restricted-value version specific to that element's requirements.
-->     <AttributeType name="id" dt:type="string"/>     <AttributeType name="lang" dt:type="string"/>     <AttributeType name="type" dt:type="string"/>     <AttributeType name="datatype" dt:type="string"/>     <!-- LINK ATTRIBUTES -->     <!-- 
· CLink: link points to a concept 
· BLink: link points to a bibliographical entry
· TLink: link points to a term 
· PLink: link points to a person
· GLink: link points to a graphics or other binary data object
· SLink: link pointing to a (non-leaf-)node of a pick-tree
· ULink: universal link points to any external entity using URL syntax
-->    <AttributeType name="Blink" dt:type="string" required="no">	          <description>Link to a bibliographic entry (stored in the same database).</description>    </AttributeType>    <AttributeType name="Clink" dt:type="string" required="no">	          <description>Link to a concept (stored in the same database). The link target is an entrynumber.</description>    </AttributeType>    <AttributeType name="Glink" dt:type="string" required="no">	          <description>Link to a graphics file (not stored in the database). The link target is a filename.</description>    </AttributeType>    <AttributeType name="Plink" dt:type="string" required="no">	          <description>Link to a user (stored in user manager). The link target is the user name (user id).</description>    </AttributeType>    <AttributeType name="Slink" dt:type="string" required="no">	          <description>Link to node in a pick-tree (Subject value).</description>    </AttributeType>    <AttributeType name="Tlink" dt:type="string" required="no">	          <description>Link to a term (stored in the same database). The link target is "index:term".</description>    </AttributeType>    <AttributeType name="Ulink" dt:type="string" required="no">	          <description>Link to a URL. The link target is specified in standard URL syntax.</description>    </AttributeType>    <!-- MULTITERM ELEMENTS (IN HIERARCHICAL ORDER) -->    <!-- start element -->    <ElementType name="mtf" content="eltOnly" order="seq" model="closed">	          <description>The root node of an MTF document. A document must contain at least one concept.
  </description>	          <element type="conceptGrp" minOccurs="1" maxOccurs="*"/>    </ElementType>    <!-- concept container -->    <ElementType name="conceptGrp" content="eltOnly" order="many" model="closed">	          <description>The container for one concept. A concept has concept-level, 
  language-independent fields, and at least one language group, which 
  contains at least one term.
  </description>	          <element type="concept" minOccurs="1" maxOccurs="1"/>	          <!-- contains concept-level info and languages -->          	<element type="system" minOccurs="0" maxOccurs="*"/>          	<element type="transacGrp" minOccurs="0" maxOccurs="*"/>          	<element type="descripGrp" minOccurs="0" maxOccurs="*"/>          	<element type="languageGrp" minOccurs="1" maxOccurs="*"/>     </ElementType>     <ElementType name="concept" content="textOnly" model="closed" dt:type="ui4">	          <description>Primary element of a conceptGrp. Content is the entry number.</description>     </ElementType>     <ElementType name="system" content="textOnly" model="closed">	          <description>Contains system-maintained information like the old entry class 
  and the approval status of a concept, language or term. 
  The type attribute can be one of "entryClass" and "status".
  </description>	          <AttributeType name="type" dt:type="enumeration" dt:values="entryClass status" required="yes">		                <description>A system tag can be of type entryClass (values 1-8, inherited from old MTW databases) 
    or type status (values: new, reviewed, approved).</description>	          </AttributeType>	          <attribute type="type" required="yes"/>    </ElementType>    <ElementType name="transacGrp" content="eltOnly" order="many" model="closed">	          <description>Contains a transaction and date, and optionally a note.</description>          	<element type="transac" minOccurs="1" maxOccurs="1"/>          	<element type="date" minOccurs="1" maxOccurs="1"/>    </ElementType>    <ElementType name="date" content="textOnly" dt:type="dateTime" model="closed">	          <description>A date in ISO-8601:1988 format, as implemented by MSXML2.</description>    </ElementType>    <ElementType name="transac" content="textOnly" model="closed">	          <description>Contains a transaction type and responsible person. The type can be one
  of origination, modification. The content of the tag is the textual representation of 
  the associated person link (Plink), i.e., the person's user id. 
  </description>	          <AttributeType name="type" dt:type="enumeration" dt:values="origination modification" required="yes">		               <description>A transac tag can be of type origination (the associated field has been created) 
    or type modification (the associated field has been modified).</description>	          </AttributeType>	          <attribute type="type" required="yes"/>	          <attribute type="Plink"/>     </ElementType>     <ElementType name="descripGrp" content="eltOnly" order="many" model="closed">	          <description>Contains a descriptive element, and optionally a source, 
  transactional info, and a note.
  </description>	          <element type="descrip" minOccurs="1" maxOccurs="1"/>          	<element type="transacGrp" minOccurs="0" maxOccurs="*"/>	          <element type="descripGrp" minOccurs="0" maxOccurs="*"/>     </ElementType>     <ElementType name="descrip" content="mixed" model="closed">	          <description>Contains a descriptive, free-text element like a definition 
  or a subject field. Content is formatted text, and the tag can carry a 
  link attribute (link to concept, term, subject tree, graphics file, URL).
  </description>	          <element type="xref" minOccurs="0" maxOccurs="*"/>	          <attribute type="type" required="yes"/>	          <attribute type="Clink"/>          	<attribute type="Glink"/>          	<attribute type="Plink"/>	          <attribute type="Slink"/>	          <attribute type="Tlink"/>	          <attribute type="Ulink"/>    </ElementType>    <ElementType name="xref" content="textOnly" model="closed">	          <description>Contains a descriptive, free-text element like a definition 
  or a subject field. Content is formatted text, and the tag can carry a 
  link attribute (link to concept, term, subject tree, graphics file, URL).
  </description>	          <attribute type="Tlink" required="yes"/>    </ElementType>    <ElementType name="languageGrp" content="eltOnly" order="many" model="closed">	          <description>The container for information about all terms in one language.</description>	          <element type="language" minOccurs="1" maxOccurs="1"/>	          <element type="transacGrp" minOccurs="0" maxOccurs="*"/>	          <element type="descripGrp" minOccurs="0" maxOccurs="*"/>          	<element type="termGrp" minOccurs="1" maxOccurs="*"/>    </ElementType>    <ElementType name="language" content="empty" order="seq">	          <description>A language specifier. The type attribute holds the "name" of the language
  as specified in the database definition, the lang attribute the locale in the form "en_us".
  </description>	          <attribute type="type" required="yes"/>	          <attribute type="lang" required="yes"/>    </ElementType>    <ElementType name="termGrp" content="eltOnly" order="many" model="closed">	<description>Groups one term and all its associated information, which can be 
  descriptions, source references, notes, and transactional information.
  </description>	          <element type="term" minOccurs="1" maxOccurs="1"/>	          <element type="transacGrp" minOccurs="0" maxOccurs="*"/>	          <element type="descripGrp" minOccurs="0" maxOccurs="*"/>   </ElementType>   <ElementType name="term" content="textOnly" model="closed">	          <description>Contains a term as plain text. Note: we have requests for storing 
  formatted terms containing sub- and superscript for mathematical and chemical formulae. 
  This should be decided soon, IMHO it's doable.
  </description>   </ElementType>
</Schema>
```


