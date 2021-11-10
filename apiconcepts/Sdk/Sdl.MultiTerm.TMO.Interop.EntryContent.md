

# 
    Sdl.MultiTerm.TMO.Interop.EntryContent class




## Name

Sdl.MultiTerm.TMO.Interop.EntryContent —          Provides programmatic access to the content of an entry.



## Description



Via this class you can retrieve the content of a particular entry, either fully or partially, e.g. only a specific indexes or descriptive fields.



## Properties
.md)
* [Content](Sdl.MultiTerm.TMO.Interop.EntryContent.Content.md): Provides programmatic access to the content of a particular entry.
* [EntryClass](Sdl.MultiTerm.TMO.Interop.EntryContent.EntryClass.md): Returns the entry class of a particular entry.
* [EntryIndexes](Sdl.MultiTerm.TMO.Interop.EntryContent.EntryIndexes.md): Provides programmatic access to the indexes contained in a particular entry.
* [Fields](Sdl.MultiTerm.TMO.Interop.EntryContent.Fields.md): Provides access to the descriptive fields of a particular entry.




## Methods

* [Refresh](Sdl.MultiTerm.TMO.Interop.EntryContent.Refresh.md): Refreshes the content of the current entry.
* [Update](Sdl.MultiTerm.TMO.Interop.EntryContent.Update.md): Updates the content of a particular entry.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;

//output entry content
Debug.WriteLine(content.Content);
Debug.WriteLine("Number of entry indexes: " + content.EntryIndexes.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryContent)

