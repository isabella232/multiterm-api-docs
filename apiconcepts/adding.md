
# Adding new Entries

To add new entries to a termbase, you first need to 'construct' the entry XML content to store in the termbase. Below you see a simplified example of what a MultiTerm XML entry can look like:


```xml
<conceptGrp>
  <system type="entryClass">1</system>
  <languageGrp>
  <language type="English" lang="EN"/>
  <termGrp>
  <term>starship</term>
  </termGrp>
  </languageGrp>
</conceptGrp>
```

For more detailed information on the MultiTerm XML format, please refer to the [MTF Schema](MTF/XMLSchemaMTF.md). To add the above entry XML as a new entry to a selected termbase, you first have to store the XML stream in a string variable, e.g.:


```cs
String entryContent = "<conceptGrp> .... </conceptGrp>"
```

Then you need to apply the **New** method to the termbase entries collection, i.e.:


```cs
Entries oEntries = oTb.Entries;
oEntries.New (entryContent, true);
```

The second parameter is a boolean parameter that indicates whether the new entry should be flagged as incomplete. An entry is considered incomplete when it lacks one or more fields that are mandatory according to the termbase definition. Note that the **New** method does *not*verify whether the entry XML content is complete according to the termbase definition or not. This means that if you want to check for completeness, you would have to implement the verification logic yourself on the client side.

Depending on the outcome of this verification you can set the boolean parameter to *true*or *false*. When implementing a quick entry function, e.g. to add new entries from MS Word to the termbase, you may set this parameter always to *true*by default. That way you can make sure that any entries added via your quick entry function can be singled out easily for post-editing using the 'Incomplete Search' of MultiTerm Workstation.

Note that the entry number is not provided in the XML content. The number will be generated automatically upon adding the entry.


