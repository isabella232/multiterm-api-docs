# Name property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Name —          Returns the name of a termbase.

## Type

String
(read)

## Index Parameters
*none*

## Description

This property can be used to return the 'nice' name of a particular termbase.

## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs[0];
Debug.Write("Termbase nice name: " + oTb.Name);
```
