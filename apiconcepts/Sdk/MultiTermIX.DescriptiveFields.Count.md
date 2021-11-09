

# 
    Count property



## Name

MultiTermIX.DescriptiveFields.Count —          Returns the number of entry-level descriptive fields.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many entry-level descriptive fields the definition of a particular termbase contains.



## Sample


```cs
TermbaseDefinition tbDef = oTb.Definition;
DescriptiveFields oDFields = tbDef.Fields;
Debug.Write("Descriptive field count: " + oDFields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20MultiTermIX.DescriptiveFields.Count)

