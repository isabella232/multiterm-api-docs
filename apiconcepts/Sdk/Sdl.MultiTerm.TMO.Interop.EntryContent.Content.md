

# 
    Content property



## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.Content —          Provides programmatic access to the content of a particular entry.



## Type

String

(read / write)



## Index Parameters
*none*


## Description



This property allows you to access, for example, the descriptive fields and index fields (i.e. languages and terms) contained in a particular entry.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select a particular entry
Entries oEntries = oTb.Entries;
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;
Debug.WriteLine("Number of entry-level descriptive fields: " + content.Fields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryContent.Content)

