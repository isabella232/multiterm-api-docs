

# 
    Entries property




## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Entries —          Provides programmatic access to the entries of a termbase.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.Entries](Sdl.MultiTerm.TMO.Interop.Entries.md)

(read)



## Index Parameters
*none*


## Description



A termbase contains a number of entries (i.e. concepts). Applying the Entries property to a Termbase object provides programmatic access to all entries of that particular termbase. You may, for example, add new entries to the specified termbase.



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

Entries oEntries = oTb.Entries;

Debug.Write("Total number of entries in termbase: " + oEntries.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.Entries)

