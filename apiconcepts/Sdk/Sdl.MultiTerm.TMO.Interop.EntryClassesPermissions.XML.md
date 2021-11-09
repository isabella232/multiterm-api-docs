

# 
    XML property



## Name

Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.XML —          Returns all entry class permissions as an XML string.



## Type

String

(read)



## Index Parameters
*none*


## Description



Via this property you can retrieve all entry class information in a consolidated XML stream. This XML output contains the entry class names as well as information on whether the currently logged-in user has read/write access to them.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;

Debug.WriteLine(oClasses.XML);




Sample output:

<entryClasses canChange='0'><entryClass id='2'><name>Internal</name><read>1</read><write>0</write></entryClass><entryClass id='3'><name>Public</name><read>1</read><write>0</write></entryClass><entryClass id='1'><name>Unspecified</name><read>1</read><write>0</write></entryClass></entryClasses>
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.XML)

