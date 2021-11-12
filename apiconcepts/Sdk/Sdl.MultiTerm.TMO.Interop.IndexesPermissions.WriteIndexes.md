# WriteIndexes property

## Name

Sdl.MultiTerm.TMO.Interop.IndexesPermissions.WriteIndexes —          Returns all indexes the currently logged-in user has write access to.

## Type

String
(read)

## Index Parameters
*none*

## Description

Via this property you can return all indexes with write permission as an XML stream.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
IndexesPermissions oIndexes = oPermissions.IndexesPermissions;
Debug.WriteLine(oIndexes.WriteIndexes);
```

Sample output:
```xml
<indexes>
    <index>
        <name locale = 'DE'>German</name>
    </index>
    <index>
        <name locale = 'EN'>English</name>
    </index>
</indexes>
```

