

# 
    Name property



## Name

Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Name —          Returns the name of a particular entry class.



## Type

String

(read)



## Index Parameters
*none*


## Description



You can use this property, e.g. to generate a list of all accessible entry classes.



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



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryClassPermissions.Name)

