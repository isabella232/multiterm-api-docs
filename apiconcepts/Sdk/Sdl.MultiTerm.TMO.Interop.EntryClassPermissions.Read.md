

# 
    Read property



## Name

Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Read —          Indicates whether the currently logged-in user has read-access to a particular class.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



This property returns true if the currently logged-in user has read-access to entries of a particular entry class. This will always be the case, for if a user can access the class, he/she at least has read-only access to it.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;

//list all available entry classes
for(int i=0;i<oClasses.Count;i++)
{
   	EntryClassPermissions oClass = oClasses[i];
   	Debug.WriteLine(oClass.Name);
   	Debug.WriteLine("Do I have read-access to this class? " + oClass.Read);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Read)

