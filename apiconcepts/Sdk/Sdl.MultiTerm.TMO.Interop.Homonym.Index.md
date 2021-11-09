

# 
    Index property



## Name

Sdl.MultiTerm.TMO.Interop.Homonym.Index —          Returns the index the homonym term was found in.



## Type

String

(read)



## Index Parameters
*none*


## Description



This property is useful for outputting the index (i.e. language) a particular homonym term belongs to.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");

//select first homonym term
Homonym oHomonym = oHomonyms[0];
Debug.Write("Homonym index: " + oHomonym.Index);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Homonym.Index)

