# Item property


## Name

Sdl.MultiTerm.TMO.Interop.Indexes.Item —          Provides access to a specific termbase index.

## Type
[Sdl.MultiTerm.TMO.Interop.Index](Sdl.MultiTerm.TMO.Interop.Index.md)
(read)

## Index Parameters

* Index (Variant)

## Description

Via this class you can access a particular index (language). You can either provide the index number, e.g. , of the actual index label, e.g. Item("English"), as parameter.

## Sample


```cs
TermbaseDefinition tbDef = oTb.Definition;
Indexes oIndexes = tbDef.Indexes;
Debug.Write(oIndexes["German"].Locale);
```



