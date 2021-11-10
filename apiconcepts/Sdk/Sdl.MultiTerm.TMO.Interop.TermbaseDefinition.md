

# 
    Sdl.MultiTerm.TMO.Interop.TermbaseDefinition class




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseDefinition —          Provides programmatic access to the termbase definition.



## Description



A termbase definition contains the indexes (i.e. languages) and descriptive fields of a termbase as well as information on the entry structure (i.e. the field hierarchy).

The TermbaseDefinition class provides programmatic access to the definition of a particular termbase. Via this class you can, for example, retrieve information such as the number of indexes and descriptive fields contained in the termbase definition, the field labels, etc.

The sample below shows how to loop through all indexes in a termbase definition and how to output the index label and locale. Moreover, the sample script loops through all descriptive fields (entry-level, index-level, and term-level fields) and returns the respective field labels.



## Properties
.md)
* [\_Schema](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition._Schema.md): Returns the schema for a termbase definition.
* [Fields](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Fields.md): Provides access to entry-level fields.
* [Indexes](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Indexes.md): Provides programmatic access to the indexes of a termbase definition.




## Methods

* [Save](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Save.md): Saves the selected termbase definition to an external file.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.StartWizard.md): Calls the Termbase Definition Wizard.




## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs["Termbase Name"];

TermbaseDefinition tbDef = oTb.Definition;
Debug.Write("Number of entry-level fields in definition: " + tbDef.Fields.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseDefinition)

