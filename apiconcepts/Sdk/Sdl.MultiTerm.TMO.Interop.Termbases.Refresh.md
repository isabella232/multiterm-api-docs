#  Refresh method

## Name

Sdl.MultiTerm.TMO.Interop.Termbases.Refresh —          Refreshes a termbase collection.

## Returntype

void

## Parameters
*none*


## Description


This method clears the termbases cache. For example, it may be useful to call this method after a new termbase has been added to update the corresponding termbase list on the client side.



## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
oTbs.Refresh();
```
