

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.PicklistValues.Count —          Returns the number of picklist values associated with a particular picklist field.



## Type

Long

(read)



## Index Parameters
*none*


## Description



This property is used to ascertain the number of picklist values associated with a particular picklist field.



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
Debug.WriteLine("Picklist field count: " + oValues.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.PicklistValues.Count)

