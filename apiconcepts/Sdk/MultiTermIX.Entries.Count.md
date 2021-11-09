

# 
    Count property



## Name

MultiTermIX.Entries.Count —          Returns the total number of termbase entries.



## Type

Long

(read)



## Index Parameters
*none*


## Description



You can use this property to ascertain the total number of entries contained in a particular termbase.



## Sample


```cs
Termbase oTb = oTbs["01test"];

Entries oEntries = oTb.Entries;
Debug.Write("Total entry count: " + oEntries.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20MultiTermIX.Entries.Count)

