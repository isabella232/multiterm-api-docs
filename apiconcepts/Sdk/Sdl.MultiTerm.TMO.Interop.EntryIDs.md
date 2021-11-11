# Sdl.MultiTerm.TMO.Interop.EntryIDs class




## Name

Sdl.MultiTerm.TMO.Interop.EntryIDs —          Provides programmatic access to the collection of entry numbers of a particular termbase.



## Description



Via this class you can, for example, list all entry numbers contained in a termbase. Entry numbers are used to uniquely identify termbase entries. Note that entries may get deleted in the course of time. This is why certain entry numbers might be 'missing' from the collection. For this reason, you cannot assume that the entry number collection is a continuous succession of numbers from 1 to n.

This class is therefore useful if you want to implement an entries iterator function.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.EntryIDs.Count.md): Returns the number of entry ids contained in a termbase.
* [Item](Sdl.MultiTerm.TMO.Interop.EntryIDs.Item.md): Refers to a particular entry id.




## Methods
*None*


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//get entry ids
EntryIDs oIds = oTb.Entries.GetEntryIDs();
for(int i=1;i==oIds.Count;i++)
{
   	Debug.WriteLine(oIds[i]);
}
```

