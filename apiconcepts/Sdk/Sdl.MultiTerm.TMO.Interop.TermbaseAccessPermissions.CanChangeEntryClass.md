#  CanChangeEntryClass property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.CanChangeEntryClass —          Returns whether the currently-logged in user can change entry class values.


## Type

Boolean
(read)


## Index Parameters
*none*

## Description

Via this property you can ascertain whether a user has the permission to change the values of entry classes, e.g. from 'Unspecified' to 'Confidential'. It returns true if the user is allowed to change entry class values, false if not.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
Debug.WriteLine(oPermissions.CanChangeEntryClass);
```
