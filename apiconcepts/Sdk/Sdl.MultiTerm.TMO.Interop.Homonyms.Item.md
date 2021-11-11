#  Item property




## Name

Sdl.MultiTerm.TMO.Interop.Homonyms.Item —          Provides access to a particular homonym.



## Type
[Sdl.MultiTerm.TMO.Interop.Homonym](Sdl.MultiTerm.TMO.Interop.Homonym.md)

(read)



## Index Parameters

* Index (Variant)




## Description



Via this property you can select a specific homonym, to retrieve the actual term, the corresponding entry id, and the index the homonym is in. The Index parameter is usually a number, for the 0-based position in the list, but can also be a string representing a term



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");

//select first homonym term
Homonym oHomonym = oHomonyms[0];
Debug.Write("Homonym term: " + oHomonym.Term);
Debug.Write("Homonym entry id: " + oHomonym.EntryID.ToString());

//select second homonym term
oHomonym = oHomonyms[1];
Debug.Write("Homonym term: " + oHomonym.Term);
Debug.Write("Homonym entry id: " + oHomonym.EntryID.ToString());
```


