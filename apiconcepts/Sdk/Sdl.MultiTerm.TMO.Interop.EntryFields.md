

# 
    Sdl.MultiTerm.TMO.Interop.EntryFields class



## Name

Sdl.MultiTerm.TMO.Interop.EntryFields —          Provides programmatic access to the entry-level fields of a particular entry.



## Description



Via this class you can retrieve the descriptive fields that refer to the entry as such, e.g. "Subject."



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.EntryFields.Count.html): Returns the number of entry-level descriptive fields.
* [Item](Sdl.MultiTerm.TMO.Interop.EntryFields.Item.html): Refers to a particular entry-level descriptive field.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.EntryFields.Add.html): Adds an entry-level descriptive field to the collection.




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

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryFields)

