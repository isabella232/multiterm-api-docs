#  Count property

## Name

Sdl.MultiTerm.TMO.Interop.IndexesPermissions.Count —          Returns the number of indexes that the currently logged-in user can access.

## Type

Long
(read)

## Index Parameters
*none*


## Description

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
IndexesPermissions oIndexes = oPermissions.IndexesPermissions;
Debug.WriteLine("Number of accessible indexes: " + oIndexes.Count.ToString());
```
