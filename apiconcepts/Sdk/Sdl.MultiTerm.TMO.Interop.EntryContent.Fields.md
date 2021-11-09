

# 
    Fields property



## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.Fields —          Provides access to the descriptive fields of a particular entry.



## Type

[Sdl.MultiTerm.TMO.Interop.EntryFields](Sdl.MultiTerm.TMO.Interop.EntryFields.html)

(read)



## Index Parameters
*none*


## Description



Entry-level descriptive fields are fields (e.g. text or picklist fields) that define the whole entry, e.g. 'Subject: Medicine'.

Via this property you can retrieve any entry-level descriptive fields, i.e. field label and content.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;

EntryFields oFields = content.Fields;
for(int i=0;i<oFields.Count;i++)
{
   	Debug.WriteLine(oFields[i].Name + ": " + oFields[i].Value);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryContent.Fields)

