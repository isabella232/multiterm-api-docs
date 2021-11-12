# Count property

## Name

Sdl.MultiTerm.TMO.Interop.Indexes.Count —          Returns the number of indexes (i.e. languages) contained in a termbase definition.

## Type

Long
(read)

## Index Parameters
*none*

## Description

## Sample


```cs
Termbase oTb = oTbs["Termbase1"];

TermbaseDefinition oDef = oTb.Definition;
Debug.WriteLine("Number of indexes: " + oDef.Indexes.Count.ToString());
```

