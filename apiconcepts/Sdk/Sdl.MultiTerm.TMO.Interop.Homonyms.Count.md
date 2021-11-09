

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.Homonyms.Count —          Returns the number of homonyms for a particular termbase index.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many homonyms a specific termbase index contains.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");
Debug.Write("Homonym count: " + oHomonyms.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Homonyms.Count)

