

# 
    EntryClasses property




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryClasses —          Provides programmatic access to the entry classes the currently logged-in user has access to.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions](Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.md)

(read)



## Index Parameters
*none*


## Description



Access to entries can be restricted using entry classes. Via this property you can determine to which entry classes the currently logged-in user has access.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["TRADOS"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;
Debug.WriteLine("Number of accessible entry classes: " + oClasses.Count.ToString());

oServerRep.Disconnect();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryClasses)

