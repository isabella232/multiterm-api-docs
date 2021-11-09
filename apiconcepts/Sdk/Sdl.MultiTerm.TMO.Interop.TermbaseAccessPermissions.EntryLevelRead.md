

# 
    EntryLevelRead property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryLevelRead —          Returns true if the currently logged-in user has read access to entry-level fields.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain whether the currently logged-in user has read access to entry-level descriptive fields, i.e. fields that are not associated with a particular index.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
Debug.WriteLine("User has read access to entry-level descriptive fields: " + oPermissions.EntryLevelRead);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryLevelRead)

