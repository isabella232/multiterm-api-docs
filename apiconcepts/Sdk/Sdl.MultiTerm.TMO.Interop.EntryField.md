

# 
    Sdl.MultiTerm.TMO.Interop.EntryField class



## Name

Sdl.MultiTerm.TMO.Interop.EntryField —          Provides programmatic access to a particular entry-level descriptive field.



## Description



Via this class, you can, for example, return the field label and/or value of a particular descriptive field, e.g. 'Subject: Medicine'.



## Properties

* [Name](Sdl.MultiTerm.TMO.Interop.EntryField.Name.html): Returns the name, i.e. the label of a particular entry-level descriptive field.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.EntryField.ReadOnly.html): Returns whether a particular entry-level descriptive field is read-only.
* [Value](Sdl.MultiTerm.TMO.Interop.EntryField.Value.html): Returns the value of a particular entry-level descriptive field.




## Methods
*None*


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
Debug.WriteLine("Field label: " + oField.Name);
Debug.WriteLine("Field value: " + oField.Value);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryField)
