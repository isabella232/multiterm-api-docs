

# 
    Merge method




## Name

Sdl.MultiTerm.TMO.Interop.Entry.Merge —          Merges the content of two entries into one.



## Returntype

void



## Parameters
.md)
* MergeWithEntry ([Sdl.MultiTerm.TMO.Interop.Entry](Sdl.MultiTerm.TMO.Interop.Entry.md))




## Description



In some cases it is useful to merge two distinct entries into one, for example, when there are two entries in the termbase that express exactly the same concept. One these entries may, for example, have an index or a descriptive field that the other one does not have. In this case it makes sense to combine the two entries into one to keep the termbase as lean and efficient as possible and to not clutter it unnecessarily with distinct entries that belong to the same concept.

Example: suppose you would like to merge the content from entry number 2 into entry number 2. To do this, you first need to Lock the entry 1, then apply the Merge method, which requires the content of entry 2 as parameter, to the entry 1 object.

Note that you need to apply the [Update](Sdl.MultiTerm.TMO.Interop.EntryContent.Update.md) method after the merge operation.

After merging entry 1 will also have the content of entry 2, which will still remain. To remove entry 2 from the termbase, you need to apply the [Delete](Sdl.MultiTerm.TMO.Interop.Entry.Delete.md) method to it.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entries to merge
Entry firstEntry = oEntries.Item(1);
Entry secondEntry = oEntries.Item(2);

//lock entry, e.g. for editing
firstEntry.LockEntry(Sdl.MultiTerm.TMO.Interop.MtLockingState.mtLock);
firstEntry.Merge(secondEntry);
firstEntry.Content.Update();
firstEntry.LockEntry(Sdl.MultiTerm.TMO.Interop.MtLockingState.mtUnlock);

//delete second (redundant) entry
secondEntry.Delete();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entry.Merge)

