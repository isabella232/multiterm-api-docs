

# 
    Sdl.MultiTerm.TMO.Interop.Homonyms class



## Name

Sdl.MultiTerm.TMO.Interop.Homonyms —          Provides programmatic access to the homonym entries of a particular termbase.



## Description



Homonyms are duplicate terms. Those can be actual duplicates, i.e. redundant terms, but it can also be the same term expressing different concepts, e.g. "book" (book for reading) and "book" (to book a flight).

Via this class you can access all homonyms (if any) contained in a termbase. As parameter you need to provide the index that should be searched for homonyms.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.Homonyms.Count.html): Returns the number of homonyms for a particular termbase index.
* [Item](Sdl.MultiTerm.TMO.Interop.Homonyms.Item.html): Provides access to a particular homonym.




## Methods
*None*


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");
Debug.Write("Homonym count: " + oHomonyms.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Homonyms)

