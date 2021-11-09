

# 
    Sdl.MultiTerm.TMO.Interop.Entry class



## Name

Sdl.MultiTerm.TMO.Interop.Entry —          Provides programmatic access to a particular entry.



## Description



This class allows you to access a particular entry, e.g. for outputting the entire entry content, for applying an entry layout, etc. Entries are programmatically selected via the unique entry id.



## Properties

* [Content](Sdl.MultiTerm.TMO.Interop.Entry.Content.html): Provides access to the content of an entry.
* [ID](Sdl.MultiTerm.TMO.Interop.Entry.ID.html): Returns the id of an entry.
* [IsComplete](Sdl.MultiTerm.TMO.Interop.Entry.IsComplete.html): Returns whether an entry is complete or not.
* [IsRtf](Sdl.MultiTerm.TMO.Interop.Entry.IsRtf.html): Returns whether an entry is RTF.
* [LockedBy](Sdl.MultiTerm.TMO.Interop.Entry.LockedBy.html): Returns the name of the user who locked the entry.




## Methods

* [ApplyExport](Sdl.MultiTerm.TMO.Interop.Entry.ApplyExport.html): Exports a particular entry.
* [ApplyFilter](Sdl.MultiTerm.TMO.Interop.Entry.ApplyFilter.html): Applies a filter definition to a specified entry and returns True or False, depending on whether the entry matches the filter.
* [ApplyLayout](Sdl.MultiTerm.TMO.Interop.Entry.ApplyLayout.html): Applies a layout definition to a MultiTerm entry XML stream.
* [Delete](Sdl.MultiTerm.TMO.Interop.Entry.Delete.html): Removes an entry from the termbase.
* [LockEntry](Sdl.MultiTerm.TMO.Interop.Entry.LockEntry.html): Locks an entry for editing.
* [Merge](Sdl.MultiTerm.TMO.Interop.Entry.Merge.html): Merges the content of two entries into one.
* [MergeEx](Sdl.MultiTerm.TMO.Interop.Entry.MergeEx.html): deprecated
* [Save](Sdl.MultiTerm.TMO.Interop.Entry.Save.html): Saves an entry to the termbase.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 and output entry content
Entry oEntry = oEntries.Item(1);
Debug.Write(oEntry.Content.Content);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entry)

