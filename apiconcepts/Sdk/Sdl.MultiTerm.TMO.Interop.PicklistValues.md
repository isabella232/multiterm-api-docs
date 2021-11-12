# Sdl.MultiTerm.TMO.Interop.PicklistValues class

## Name

Sdl.MultiTerm.TMO.Interop.PicklistValues —          Provides programmatic access to the picklist values of a picklist type descriptive field.

## Description


The termbase creators/administrators can define descriptive fields to be of the type picklist. Any such fields are associated with a list of values (at least one value is required), which are specified in the termbase definition.

When adding or editing such fields later on, the user is required to select one (or several) pre-defined picklist values rather than entering free text information. This ensures consistency of the values for particular fields throughout the termbase.

Examples for picklist fields are "Subject", "Product type", "Department", "Gender", "Grammar information", etc.

An example application for this class is filling a drop-down list with the picklist values of a particular field.


## Properties
* [Count](Sdl.MultiTerm.TMO.Interop.PicklistValues.Count.md): Returns the number of picklist values associated with a particular picklist field.
* [Item](Sdl.MultiTerm.TMO.Interop.PicklistValues.Item.md): Refers to a specific value from the picklist of a specified picklist field.


## Methods
*None*


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//access termbase definition
TermbaseDefinition oDef = oTb.Definition;
//select first descriptive field
DescriptiveField oField = oDef.Fields[0];
//generate list of picklist values
PicklistValues oValues = oField.PicklistValues;
for(int i=0;i<oValues.Count;i++)
{
   	Debug.WriteLine(oValues[i]);
}
```
