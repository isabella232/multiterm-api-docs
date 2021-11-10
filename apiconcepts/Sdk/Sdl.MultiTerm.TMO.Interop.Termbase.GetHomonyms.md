

# 
    GetHomonyms method




## Name

Sdl.MultiTerm.TMO.Interop.Termbase.GetHomonyms —          Retrieves all homonym entries of a particular termbase.



## Returntype
.md)
[Sdl.MultiTerm.TMO.Interop.Homonyms](Sdl.MultiTerm.TMO.Interop.Homonyms.md)



## Parameters

* Index (String)
* Source (String)
* Target (String)




## Description



Homonyms are duplicate terms. Those can be actual duplicates, i.e. redundant terms, but it can also be the same term expressing different concepts, e.g. "book" (book for reading) and "book" (to book a flight).

Via this class you can access all homonyms (if any) contained in a termbase. As parameter you need to provide the index that should be searched for homonyms.

The Source and Target parameters are only used if you have set an active filter for the termbase, and the filter is using "Source" or "Target" in a condition instead of actual index name. If you don't use such a filter you can set these parameters to "" (empty string).



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

Sdl.MultiTerm.TMO.Interop.Homonyms oDoubles = oTb.GetHomonyms("English", "English", "German");
Debug.Write("Homonym count in English index: " + oDoubles.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.GetHomonyms)

