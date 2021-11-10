

# 
    Indexes property




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Indexes —          Provides programmatic access to the indexes of a termbase definition.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.Indexes](Sdl.MultiTerm.TMO.Interop.Indexes.md)

(read)



## Index Parameters
*none*


## Description



Each termbase definition contains at least one index (i.e. a language). The termbase creator/administrator adds the indexes from a list of available languages when setting up (or editing) the termbase definition.

Each index is automatically assigned a locale (e.g. "EN-US"). The termbase creator/administrator can assign a custom label to each index, by which it is uniquely identified. Via this class you can, for example, you can retrieve index labels and locales.



## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs[0];

TermbaseDefinition tbDef = oTb.Definition;
Debug.Write("Number of index fields in definition: " + tbDef.Indexes.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Indexes)

