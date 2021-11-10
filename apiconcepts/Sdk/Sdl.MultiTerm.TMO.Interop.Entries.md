

# 
    Sdl.MultiTerm.TMO.Interop.Entries class




## Name

Sdl.MultiTerm.TMO.Interop.Entries —          Provides programmatic access to the entries in a termbase.



## Description



A termbase is a collection of entries (i.e. concepts). Via this class you can, for example, add new entries to the specified termbase, or select a specific entry by using its unique concept number, etc.



## Properties
.md
* [Count](Sdl.MultiTerm.TMO.Interop.Entries.Count.md): Returns the total number of termbase entries.




## Methods

* [ActiveFilterHasChanged](Sdl.MultiTerm.TMO.Interop.Entries.ActiveFilterHasChanged.md): Returns true if the active filter has changed, otherwise false.
* [GetCrossLinkedEntry](Sdl.MultiTerm.TMO.Interop.Entries.GetCrossLinkedEntry.md: Allows you to retrieve the content of a cross-linked entry.
* [GetEntryIDs](Sdl.MultiTerm.TMO.Interop.Entries.GetEntryIDs.md: Retrieves all entry ids contained in a termbase.
* [Item](Sdl.MultiTerm.TMO.Interop.Entries.Item.md: Refers to a particular entry.
* [New](Sdl.MultiTerm.TMO.Interop.Entries.New.md: Adds a new entry to the termbase.
* [ReloadLayout](Sdl.MultiTerm.TMO.Interop.Entries.ReloadLayout.md): Refreshes the entry layout.
* [ReloadTermbaseDefinition](Sdl.MultiTerm.TMO.Interop.Entries.ReloadTermbaseDefinition.md): Refreshes the current termbase definition.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Entries oEntries = oTb.Entries;
Debug.Write("Total entry count: " + oEntries.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entries)

