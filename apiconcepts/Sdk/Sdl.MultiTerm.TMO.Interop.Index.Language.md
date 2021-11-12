# Language property

## Name

Sdl.MultiTerm.TMO.Interop.Index.Language —          Returns the English name of the index language.

## Type

String
(read)


## Index Parameters
*none*


## Description

See [Label](Sdl.MultiTerm.TMO.Interop.Index.Label.md)

## Sample


```cs
Termbase oTb = oTbs["Termbase1"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
Debug.WriteLine(oIndex.Language);
```


