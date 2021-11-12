# Count property
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
