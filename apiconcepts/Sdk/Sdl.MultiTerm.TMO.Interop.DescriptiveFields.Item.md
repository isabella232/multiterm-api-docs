

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Item —          Provides access to a particular entry-level descriptive fields.



## Type

[Sdl.MultiTerm.TMO.Interop.DescriptiveField](Sdl.MultiTerm.TMO.Interop.DescriptiveField.html)

(read)



## Index Parameters

* Index (Variant)




## Description



To select a particular field you can either provide the index number, e.g. Item(0) or the actual field label, e.g. Item("Subject") as parameter.



## Sample


```cs
TermbaseDefinition tbDef = oTb.Definition;
DescriptiveFields oDFields = tbDef.Fields;
//select first descriptive field
DescriptiveField oDField = oDFields[0];
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Item)

