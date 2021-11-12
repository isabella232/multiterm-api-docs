# Item property

## Name

Sdl.MultiTerm.TMO.Interop.IndexesPermissions.Item —          Refers to a particular index permission.

## Type
[Sdl.MultiTerm.TMO.Interop.IndexPermissions](Sdl.MultiTerm.TMO.Interop.IndexPermissions.md)
(read)

## Index Parameters

* Index (Variant)

## Description

You can use this property, for example, to return the label of a particular index the currently logged-in user has access to and see whether the user has read-only or read/write access to it.


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
IndexesPermissions oIndexes = oPermissions.IndexesPermissions;
for(int i=0;i<oIndexes.Count;i++)
{
   	IndexPermissions oIndex = oIndexes[i];
   	Debug.WriteLine(oIndex.Label);
}
```
