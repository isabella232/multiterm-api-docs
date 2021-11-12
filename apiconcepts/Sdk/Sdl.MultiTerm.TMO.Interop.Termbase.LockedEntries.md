# LockedEntries property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.LockedEntries —          Provides programmatic access to the locked entries of a termbase.

## Type
[Sdl.MultiTerm.TMO.Interop.LockedEntries](Sdl.MultiTerm.TMO.Interop.LockedEntries.md)
(read)


## Index Parameters
*none*

## Description

An entry is locked when a user is in the process of editing it. This is to prevent other users from gaining write-access to the same entry and trying to edit it as well. Via this property you can gain programmatic access to all locked termbase entries, e.g. to retrieve a list of all locked entries.


## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

LockedEntries oLockedEntries = oTb.LockedEntries;

Debug.Write("Total number of locked entries in termbase: " + oLockedEntries.Count.ToString());
```

