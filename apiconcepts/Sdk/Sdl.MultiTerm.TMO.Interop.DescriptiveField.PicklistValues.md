

# 
    PicklistValues property



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.PicklistValues —          Provides access to the picklist values of a picklist field.



## Type

[Sdl.MultiTerm.TMO.Interop.PicklistValues](Sdl.MultiTerm.TMO.Interop.PicklistValues.html)

(read)



## Index Parameters
*none*


## Description



Descriptive fields that have the field type "picklist" are associated with a number of values that are defined by the termbase creator/administrator in the termbase definition. This ensures consistent use of the field values when new entries are created (e.g. "Subject -&gt; Engineering, Medicine, Biology").

This property is used to access the picklist values associated with a particular field.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
PicklistValues oValues = oField.PicklistValues;
Debug.WriteLine("Picklist value count: " + oValues.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveField.PicklistValues)

