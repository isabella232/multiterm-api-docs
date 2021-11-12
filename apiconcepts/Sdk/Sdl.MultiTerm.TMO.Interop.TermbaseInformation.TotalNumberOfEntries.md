#  TotalNumberOfEntries property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.TotalNumberOfEntries —          Returns the total entry count for the specified termbase.

## Type

Long
(read)

## Index Parameters
*none*

## Description

This property is used to retrieve the total number of entries contained in a specific termbase.

## Sample

```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Total number of termbase entries: " + tbInfo.TotalNumberOfEntries.ToString());
```
