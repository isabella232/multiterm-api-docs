

# 
    New method



## Name

Sdl.MultiTerm.TMO.Interop.Entries.New —          Adds a new entry to the termbase.



## Returntype

[Sdl.MultiTerm.TMO.Interop.Entry](Sdl.MultiTerm.TMO.Interop.Entry.html)



## Parameters

* EntryXML (String)
* Incomplete (Boolean)




## Description



By applying this method to an Entries collection you add a new entry to a selected termbase. This method requires the new entry content as an XML stream.

Below is a (highly simplified) example of what a MultiTerm XML stream looks like. Note that entries for server termbases require an entry class, which is not the case for locally stored termbases.

&lt;conceptGrp&gt; &lt;system type="entryClass"&gt;1&lt;/system&gt; &lt;languageGrp&gt; &lt;language type="English" lang="EN"/&gt; &lt;termGrp&gt; &lt;term&gt;starship&lt;/term&gt; &lt;/termGrp&gt; &lt;/languageGrp&gt; &lt;/conceptGrp&gt;

The second parameter is a boolean parameter that indicates whether the new entry should be flagged as incomplete. An entry is incomplete when it lacks a field that is mandatory according to the termbase definition. This method does not verify whether the entry XML stream is complete or not. You would have to implement that logic yourself. Depending on the outcome of this verification you can set this parameter to true or false. When implementing a quick entry function, e.g. to add new entries from MS Word to the termbase, you may set this parameter always to true by default. In this case all entries added via your quick entry function can be singled out easily for post-editing using the 'Incomplete Search' of MultiTerm Workstation.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//define new entry content
String entryContent="<conceptGrp><system type='entryClass'>1</system>";
entryContent+="<languageGrp><language type='English' lang='EN'/>";
entryContent+="<termGrp><term>starship</term></termGrp></languageGrp></conceptGrp>";
//add new entry and flag as incomplete
oEntries.New(entryContent, true);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entries.New)

