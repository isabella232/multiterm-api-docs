

# 
    Refresh method



## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.Refresh —          Refreshes the content of the current entry.



## Returntype

void



## Parameters
*none*


## Description



You can apply this method to make sure that the user always sees the most up-to-date entry content, e.g. when one user is viewing an entry that has just been updated by another user.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);

//refresh entry content
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryContent.Refresh)

