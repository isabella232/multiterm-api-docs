

# 
    Label property



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveField.Label —          Returns the field label.



## Type

String

(read)



## Index Parameters
*none*


## Description



Descriptive field labels are fully user-definable, i.e. the termbase creator/administrator determines the name of the fields that are added to the termbase definition, e.g. "Example", "Context", "Subject", "Note", etc.

Via this property you can retrieve the label of a particular field



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

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveField.Label)

