# CreationDate property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.CreationDate —          Returns the termbase creation date.

## Type

String
(read)

## Index Parameters
*none*

## Description

This property is used to retrieve the creation date of a specified termbase.

## Sample

```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Termbase creation date: " + tbInfo.CreationDate);
```


