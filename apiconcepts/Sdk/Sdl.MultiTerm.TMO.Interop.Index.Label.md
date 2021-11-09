

# 
    Label property



## Name

Sdl.MultiTerm.TMO.Interop.Index.Label —          Returns the label of a particular index.



## Type

String

(read)



## Index Parameters
*none*


## Description



The label is the name of the index which is used to uniquely identify an index, i.e. a language, e.g. "English." Labels are fully user-definable.



## Sample


```cs
Termbase oTb = oTbs["Termbase1"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
Debug.WriteLine(oIndex.Label);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Index.Label)

