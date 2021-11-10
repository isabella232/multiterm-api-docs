
# Schema Attributes Reference

<dl class="dl">		  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-E782DE6B-80A8-4205-A70C-678633CC592A">open model	  </dt>
	  <dd class="dd">The element can contain elements, attributes, and text not specified in the content model. This is the default value. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-83C99CAE-E4D2-41AC-80A4-3A25E1734968">closed model	  </dt>
	  <dd class="dd">The element cannot contain elements, attributes, and text except for that specified in the content model. DTDs use a closed model. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-4FA7AE9C-8DD5-4E89-AF74-C6E19065AA5E">textOnly content	  </dt>
	  <dd class="dd">The element can contain only text, not elements. Note that if the model attribute is set to "open", the element can contain text and additional elements.	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-5286741B-5821-43CF-9105-3604EC331274">eltOnly content	  </dt>
	  <dd class="dd">The element can contain only the elements, not free text. Note that if the model attribute is set to "open", the element can contain text and additional elements.	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-FA08BF40-B7BC-4F5C-8561-39CA8CC069FC">empty content	  </dt>
	  <dd class="dd">The element cannot contain text or elements. Note that if the model attribute is set to "open", the element can contain text and additional elements. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-EB52FE80-7522-4598-A066-D7C49CA85545">mixed content	  </dt>
	  <dd class="dd">The element can contain a mix of named elements and text. This is the default value. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-9BB17F57-F975-4AF9-ADB2-053A5140F0A0">one order	  </dt>
	  <dd class="dd">Permits only one of a set of elements. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-9C814F30-C1BB-4C05-B5E2-A89996B83A81">seq order	  </dt>
	  <dd class="dd">Requires the elements to appear in the specified sequence. 	  </dd>
			  <dt class="dt dlterm" id="GUID-267CBDE0-2132-4192-ABAE-F683BE77335F__GUID-388E535B-D98A-40F6-B218-872E39079A0D">many order	  </dt>
	  <dd class="dd">Permits the elements to appear (or not appear) in any order. This is the default. 	  </dd>
	 </dl>


