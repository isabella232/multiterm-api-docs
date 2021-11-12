#  Count property

## Name

Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.Count —          Returns the number of entry classes a user has access to.

## Type
Long
(read)

## Index Parameters
*none*

## Description


## Sample


```cs
//select termbase
Termbase oTb = oTbs["TRADOS"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;
Debug.WriteLine("Number of accessible entry classes: " + oClasses.Count.ToString());

oServerRep.Disconnect();
```
