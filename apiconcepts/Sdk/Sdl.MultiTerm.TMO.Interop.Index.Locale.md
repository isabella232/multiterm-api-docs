

# 
    Locale property



## Name

Sdl.MultiTerm.TMO.Interop.Index.Locale —          Returns the locale of the index.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each index is associated with a standard locale, e.g. "EN" or "EN-US", etc.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
Debug.WriteLine(oIndex.Locale);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Index.Locale)

