#  ChangeDate property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.ChangeDate —          Returns the last termbase change date.

## Type

Date
(read)


## Index Parameters
*none*

## Description

Returns the date of the last change made to the specified termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Debug.Write("Termbase change date: " + oTb.ChangeDate);
```

