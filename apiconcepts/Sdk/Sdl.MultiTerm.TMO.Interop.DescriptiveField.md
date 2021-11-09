

# 
    Sdl.MultiTerm.TMO.Interop.DescriptiveField class



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField —          Provides programmatic access to a particular descriptive field specified in a termbase definition.



## Description



Descriptive fields contain fully user-defined information to further define an entry, an index or a particular term. Examples for descriptive fields are as follows: "Definition", "Note", "Usage example", "Subject", etc.

Via the this class you can retrieve various information on a particular descriptive field that was added by the termbase creator/administrator to the termbase definition, e.g. the field label/value, information on whether the field is multiple and/or mandatory, the field level (i.e. entry-level, index-level, or term-level), the field type (i.e. text field, picklist field, multimedia field...), etc.

A concrete application for this class would, for example, be filling a drop-down list with the labels of the available entry-level descriptive fields.



## Properties

* [Label](Sdl.MultiTerm.TMO.Interop.DescriptiveField.Label.html): Returns the field label.
* [Level](Sdl.MultiTerm.TMO.Interop.DescriptiveField.Level.html): Returns the descriptive field level value.
* [Mandatory](Sdl.MultiTerm.TMO.Interop.DescriptiveField.Mandatory.html): Returns whether the specified field is mandatory.
* [Multiple](Sdl.MultiTerm.TMO.Interop.DescriptiveField.Multiple.html): Returns whether a field can be multiple.
* [PicklistValues](Sdl.MultiTerm.TMO.Interop.DescriptiveField.PicklistValues.html): Provides access to the picklist values of a picklist field.
* [Type](Sdl.MultiTerm.TMO.Interop.DescriptiveField.Type.html): Returns the descriptive field type.




## Methods
*None*


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//list entry-level descriptive fields containted in the termbase definition
for(int i=0;i<oDef.Fields.Count;i++)
{
   	DescriptiveField thisField = oDef.Fields[i];
   	Debug.WriteLine(thisField.Label);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveField)

