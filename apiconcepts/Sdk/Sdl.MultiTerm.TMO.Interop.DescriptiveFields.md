

# 
    Sdl.MultiTerm.TMO.Interop.DescriptiveFields class



## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveFields —          Provides programmatic access to the descriptive fields of a termbase definition.



## Description



You can use this class, for example, to generate a list of all entry-level descriptive fields of a particular termbase definition.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Count.html): Returns the number of entry-level descriptive fields.
* [Item](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Item.html): Provides access to a particular entry-level descriptive fields.




## Methods
*None*


## Sample


```cs
TermbaseDefinition tbDef = oTb.Definition;
DescriptiveFields oDFields = tbDef.Fields;
Debug.Write("Descriptive field count: " + oDFields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.DescriptiveFields)

