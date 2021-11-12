# Definition property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Definition —          Provides programmatic access to a termbase definition.


## Type
[Sdl.MultiTerm.TMO.Interop.TermbaseDefinition](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.md)
(read)

## Index Parameters
*none*

## Description

A termbase definition contains the indexes (i.e. languages) and descriptive fields as well as information the entry structure (i.e. the field hierarchy).

By applying the Definition property to a termbase object you can, for example, retrieve information such as the number of indexes and descriptive fields contained in the termbase definition, the field labels, etc.

## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

TermbaseDefinition oDef = oTb.Definition;
Debug.Write("Number of languages in termbase definition: " + oDef.Indexes.Count.ToString());
```
