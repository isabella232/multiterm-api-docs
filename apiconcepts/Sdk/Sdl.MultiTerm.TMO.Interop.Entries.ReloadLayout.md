#  ReloadLayout method

## Name

Sdl.MultiTerm.TMO.Interop.Entries.ReloadLayout —          Refreshes the entry layout.


## Returntype
void


## Parameters
*none*


## Description

Applying this method to an Entries collection refreshes the entry layout. That way you can make sure that always the most current layout is applied to the entry display, e.g. when layouts are edited while you search the termbase.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

oEntries.ReloadLayout();
```

