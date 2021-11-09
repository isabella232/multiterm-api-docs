

# 
    LockedBy property



## Name

Sdl.MultiTerm.TMO.Interop.Entry.LockedBy —          Returns the name of the user who locked the entry.



## Type

String

(read)



## Index Parameters
*none*


## Description



When a user edits an entry it is locked for all other users, i.e. no one else can obtain write access to this particular entry. Via this property you can determine the name of the user who has locked a particular entry. This name corresponds to the login name the user entered in his/her client application.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);
Debug.Write("Entry locked by user " + oEntry.LockedBy);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entry.LockedBy)

