

# 
    Sdl.MultiTerm.TMO.Interop.FilterDefinition class




## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition —          Provides programmatic access to a particular filter definition.



## Description



Filters contain an XPATH statement that gets applied to the MultiTerm entries, which are XML-based. If the XPATH statement fits the entry content, it returns true, if not it returns false. Via this class you can retrieve information on a particular filter, e.g. the filter description, the content (i.e. the filter source code'), etc. In addition you can also use this class to edit an existing filter using the filter wizard.



## Properties
.md)
* [Active](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Active.md): Activates a particular filter.
* [Content](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Content.md): Returns the filter definition content.
* [Description](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Description.md): Returns the filter description.
* [ID](Sdl.MultiTerm.TMO.Interop.FilterDefinition.ID.md): Returns the unique id of the filter.
* [Name](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Name.md): Returns the name of the filter.
* [Owner](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Owner.md): Returns the owner name for a particular filter definition.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.FilterDefinition.ReadOnly.md): Returns whether a particular filter is read-only.




## Methods

* [Delete](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Delete.md): Removes the filter from the collection.
* [Load](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Load.md): Updates the selected filter from an external filter definition file.
* [Save](Sdl.MultiTerm.TMO.Interop.FilterDefinition.Save.md):  Saves the filter definition to an external file.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.FilterDefinition.StartWizard.md): Calls up the filter wizard for editing a particular filter.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

Debug.WriteLine(oFilter.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition)

