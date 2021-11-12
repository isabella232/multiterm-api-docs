#   Name property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Name —          Returns the (nice) name of a termbase.


## Type

String
(read)

## Index Parameters
*none*

## Description

This property is used to retrieve the name of the termbase.

## Sample


```cs
Termbase oTb = oTbs[0];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Termbase name: " + tbInfo.Name);
```

