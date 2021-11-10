

# 
    GetEntryIDs method




## Name

Sdl.MultiTerm.TMO.Interop.Entries.GetEntryIDs —          Retrieves all entry ids contained in a termbase.



## Returntype
.md
[Sdl.MultiTerm.TMO.Interop.EntryIDs](Sdl.MultiTerm.TMO.Interop.EntryIDs.md)



## Parameters
*none*


## Description



You can make use of this method to retrieve all entry ids of a termbase and then iterate through all termbase entries. That way you can make sure that you only iterate through entry numbers that actually exist in your termbase. Note that entry numbers might be 'missing' due to deletion of entries. For example, a termbase might contain the following entry ids: '1, 2, 5, 7'.

If you just built your iteration to go from 1 to 7, the loop will throw an error, as some entry ids no longer exist in the termbase.

Note that the entry id collection starts at 1, not 0.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//retrieve entry ids 
EntryIDs oIds = oEntries.GetEntryIDs();

for(int i=1;i<oIds.Count;i++)
{
   	Debug.WriteLine(oIds[i]);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entries.GetEntryIDs)

