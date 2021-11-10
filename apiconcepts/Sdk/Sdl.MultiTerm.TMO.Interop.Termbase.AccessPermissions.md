

# 
    AccessPermissions property




## Name

Sdl.MultiTerm.TMO.Interop.Termbase.AccessPermissions —          Provides programmatic access to the permissions the currently logged-in user has to a termbase.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.md)

(read)



## Index Parameters
*none*


## Description



Users usually have different permissions for using a termbase. For example, a particular user may have read-only permissions or may not be allowed to change entry class values. Via this class you can determine the respective user's access permissions and, e.g., output a message when the user tries to perform an action that he/she is not allowed to take such as changing an entry class value.



## Sample


```cs
Termbase oTb = oTbs["01test"];

TermbaseAccessPermissions oTbPermissions = oTb.AccessPermissions;
Debug.Write("User can change entry class values: " + oTbPermissions.CanChangeEntryClass);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.AccessPermissions)

