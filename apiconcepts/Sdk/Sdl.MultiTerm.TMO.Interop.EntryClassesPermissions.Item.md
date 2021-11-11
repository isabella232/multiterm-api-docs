# Item property

## Name

Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.Item —          Refers to a specific entry class.



## Type
[Sdl.MultiTerm.TMO.Interop.EntryClassPermissions](Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.md)
(read)

## Index Parameters

* Index (Variant)

## Description

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;

//select the first accessible entry class
EntryClassPermissions oClass = oClasses[0];
Debug.WriteLine(oClass.Name);
```

