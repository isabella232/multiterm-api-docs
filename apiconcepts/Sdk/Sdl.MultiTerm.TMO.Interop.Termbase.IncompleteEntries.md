# IncompleteEntries property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.IncompleteEntries —          Provides programmatic access to the incomplete entries of a termbase.

## Type
[Sdl.MultiTerm.TMO.Interop.IncompleteEntries](Sdl.MultiTerm.TMO.Interop.IncompleteEntries.md)
(read)


## Index Parameters
*none*


## Description

Incomplete entries are those entries that lack a field which is mandatory as per the respective termbase definition. For example, if the termbase definition imposes "Subject" as a mandatory field and this field is missing in an entry, it is considered incomplete. You may use this class to, e.g. ascertain the total number of incomplete entries of a termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

IncompleteEntries oIncompletes = oTb.IncompleteEntries;

Debug.Write("Total number of incomplete entries in termbase: " + oIncompletes.Count.ToString());
```

