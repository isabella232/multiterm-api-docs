

# 
    Sdl.MultiTerm.TMO.Interop.IndexPermissions class




## Name

Sdl.MultiTerm.TMO.Interop.IndexPermissions —          Provides programmatic access to the permissions of a particular index.



## Description



Via this class you can determine, for example, the label of a particular index that the currently logged-in user is allowed to access and see whether the user has read-only or read/write access to it.



## Properties
.md)
* [Label](Sdl.MultiTerm.TMO.Interop.IndexPermissions.Label.md): Returns the label of a particular index the currently logged-in user can access.
* [Read](Sdl.MultiTerm.TMO.Interop.IndexPermissions.Read.md): Returns true if the user has read access to this index (will always be the case).
* [Write](Sdl.MultiTerm.TMO.Interop.IndexPermissions.Write.md): Returns true if the currently logged-in user has write access to a particular index, otherwise false.




## Methods
*None*


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
   	Debug.WriteLine("Read access: " + oIndex.Read);
   	Debug.WriteLine("Write access: " + oIndex.Write);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IndexPermissions)

