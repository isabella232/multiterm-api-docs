# Label property

## Name

Sdl.MultiTerm.TMO.Interop.IndexPermissions.Label —          Returns the label of a particular index the currently logged-in user can access.

## Type

String
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
for(int i=0;i<oIndexes.Count;i++)
{
   	IndexPermissions oIndex = oIndexes[i];
   	Debug.WriteLine(oIndex.Label);
}
```