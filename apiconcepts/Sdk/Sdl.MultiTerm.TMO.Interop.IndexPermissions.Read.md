# Read property

## Name

Sdl.MultiTerm.TMO.Interop.IndexPermissions.Read —          Returns true if the user has read access to this index (will always be the case).

## Type

Boolean
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
   	Debug.WriteLine("Read access: " + oIndex.Read);
}
```