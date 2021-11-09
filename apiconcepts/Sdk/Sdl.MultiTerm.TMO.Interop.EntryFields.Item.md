

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.EntryFields.Item —          Refers to a particular entry-level descriptive field.



## Type

[Sdl.MultiTerm.TMO.Interop.EntryField](Sdl.MultiTerm.TMO.Interop.EntryField.html)

(read)



## Index Parameters

* Index (Variant)




## Description



This property is used, for example, to retrieve the field label and/or value.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select a particular entry
Entries oEntries = oTb.Entries;
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;
EntryFields oFields = content.Fields;
EntryField oField = oFields[0];
Debug.WriteLine(oField.Value);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryFields.Item)

