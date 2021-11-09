

# 
    EntryClass property



## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.EntryClass —          Returns the entry class of a particular entry.



## Type

String

(read)



## Index Parameters
*none*


## Description



You can use this property to output the entry class of the selected entry. Note that only server termbases have an entry class.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;

//output entry content
Debug.WriteLine(content.EntryClass);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryContent.EntryClass)

