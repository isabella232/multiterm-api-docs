

# 
    ReadIndexes property



## Name

Sdl.MultiTerm.TMO.Interop.IndexesPermissions.ReadIndexes —          Returns all indexes that the currently logged-in user has read-access too.



## Type

String

(read)



## Index Parameters
*none*


## Description



Via this property you can return all read-only indexes as an XML stream.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
IndexesPermissions oIndexes = oPermissions.IndexesPermissions;
Debug.WriteLine(oIndexes.ReadIndexes);



Sample output:

<indexes><index><name locale = 'DE'>German</name></index><index><name locale = 'EN'>English</name></index></indexes>
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IndexesPermissions.ReadIndexes)

