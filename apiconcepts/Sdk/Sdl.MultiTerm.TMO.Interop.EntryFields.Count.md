

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.EntryFields.Count —          Returns the number of entry-level descriptive fields.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many entry-level descriptive fields an entry has, i.e. fields that refer to the entry as such, e.g. 'Subject', 'Project', etc.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select a particular entry
Entries oEntries = oTb.Entries;
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;
EntryFields oFields = content.Fields;
Debug.WriteLine(oFields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryFields.Count)

