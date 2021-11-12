#  IndexesPermissions property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.IndexesPermissions —          Provides access to the indexes that the currently logged-in user can access.

## Type
[Sdl.MultiTerm.TMO.Interop.IndexesPermissions](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.md)
(read)

## Index Parameters
*none*

## Description

Via this class you can, for example, generate a list of all indexes that the currently logged-in user can access. In addition, you can also ascertain whether the user has read/write access to a particular index.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
IndexesPermissions oIndexes = oPermissions.IndexesPermissions;
for(int i=0;i<oIndexes.Count;i++)
{
   	Debug.WriteLine(oIndexes[i].Label);
}
```

