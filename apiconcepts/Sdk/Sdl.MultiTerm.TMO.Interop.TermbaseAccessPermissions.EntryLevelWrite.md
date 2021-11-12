# EntryLevelWrite property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryLevelWrite —          Returns true if the currently logged-in user has write access to entry-level fields.

## Type

Boolean
(read)

## Index Parameters
*none*

## Description

Via this property you can ascertain whether the currently logged-in user has write access to entry-level descriptive fields, i.e. fields that are not associated with a particular index.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
Debug.WriteLine("User has write access to entry-level descriptive fields: " + oPermissions.EntryLevelWrite);
```
