# Count property

## Name

Sdl.MultiTerm.TMO.Interop.IncompleteEntries.Count —          Returns the number of incomplete entries contained in a termbase.

## Type

Long
(read)

## Index Parameters
*none*

## Description

Via this property you can ascertain the number of incomplete entries in your termbase.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//get incomplete entries
IncompleteEntries oIncompletes = oTb.IncompleteEntries;
Debug.WriteLine("Number of incomplete entries: " + oIncompletes.Count.ToString());
```
