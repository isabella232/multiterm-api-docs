

# 
    Write property



## Name

Sdl.MultiTerm.TMO.Interop.IndexPermissions.Write —          Returns true if the currently logged-in user has write access to a particular index, otherwise false.



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
   	Debug.WriteLine("Write access: " + oIndex.Write);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IndexPermissions.Write)

