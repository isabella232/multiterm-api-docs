

# 
    Sdl.MultiTerm.TMO.Interop.EntryContent class



## Name

Sdl.MultiTerm.TMO.Interop.EntryContent —          Provides programmatic access to the content of an entry.



## Description



Via this class you can retrieve the content of a particular entry, either fully or partially, e.g. only a specific indexes or descriptive fields.



## Properties

* [Content](Sdl.MultiTerm.TMO.Interop.EntryContent.Content.html): Provides programmatic access to the content of a particular entry.
* [EntryClass](Sdl.MultiTerm.TMO.Interop.EntryContent.EntryClass.html): Returns the entry class of a particular entry.
* [EntryIndexes](Sdl.MultiTerm.TMO.Interop.EntryContent.EntryIndexes.html): Provides programmatic access to the indexes contained in a particular entry.
* [Fields](Sdl.MultiTerm.TMO.Interop.EntryContent.Fields.html): Provides access to the descriptive fields of a particular entry.




## Methods

* [Refresh](Sdl.MultiTerm.TMO.Interop.EntryContent.Refresh.html): Refreshes the content of the current entry.
* [Update](Sdl.MultiTerm.TMO.Interop.EntryContent.Update.html): Updates the content of a particular entry.




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

