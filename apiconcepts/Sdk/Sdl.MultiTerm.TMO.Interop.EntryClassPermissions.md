# Sdl.MultiTerm.TMO.Interop.EntryClassPermissions class

## Name

Sdl.MultiTerm.TMO.Interop.EntryClassPermissions —          Provides access to a particular entry class.



## Description


You can use this class, for example, to retrieve the name of a specific entry class and ascertain whether the currently logged-in user has read-only or read/write access to entries of a particular class.



## Properties

* [Name](Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Name.md): Returns the name of a particular entry class.
* [Read](Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Read.md): Indicates whether the currently logged-in user has read-access to a particular class.
* [Write](Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Write.md): Indicates whether the currently logged-in user has write-access to a class.


## Methods
*None*


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
}
```

