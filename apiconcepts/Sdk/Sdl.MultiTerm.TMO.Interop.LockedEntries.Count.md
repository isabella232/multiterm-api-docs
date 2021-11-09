

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.LockedEntries.Count —          Returns the number of locked entries.



## Type

Long

(read)



## Index Parameters
*none*


## Description



You can use this property to ascertain how many entries (if any) are currently locked in the termbase.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LockedEntries oLocks = oTb.LockedEntries;
Debug.Write("Number of locked entries: " + oLocks.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LockedEntries.Count)

