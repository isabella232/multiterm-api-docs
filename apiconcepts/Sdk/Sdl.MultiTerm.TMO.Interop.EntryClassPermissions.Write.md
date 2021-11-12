#  Write property

## Name

Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Write —          Indicates whether the currently logged-in user has write-access to a class.

## Type
Boolean
(read)

## Index Parameters
*none*

## Description

This property returns true, if the currently logged-in user has write access to entries of a particular entry class, otherwise it returns false.

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
   	Debug.WriteLine("Do I have write-access to this class? " + oClass.Write);
}
```

