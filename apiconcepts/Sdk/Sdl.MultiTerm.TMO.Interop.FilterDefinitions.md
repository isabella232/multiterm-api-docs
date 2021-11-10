

# 
    Sdl.MultiTerm.TMO.Interop.FilterDefinitions class




## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinitions —          Provides programmatic access to the filter definitions of a termbase.



## Description



Filters are used to select a subset of termbase entries, e.g. all entries that have a "Definition" field. Filters are basically XPath statements that are applied to the entry XML content.

Via this property you can, for example, return the number of available filter definitions, generate a list containing the names of available filter definitions, etc.



## Properties
.md)
* [Count](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Count.md): Returns the number of available filter definitions.
* [Item](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Item.md): Provides access to a particular filter definition.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Add.md): Adds a new filter definition to the collection.
* [Refresh](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Refresh.md): Updates the filter definition collection.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.StartWizard.md): Starts the Filter Definition wizard.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oFilters = oTb.FilterDefinitions;
Debug.Write("Number of filters: +" + oFilters.Count);

for(int i=0;i<oFilters.Count;i++)
{
   	Debug.Write(oFilters[i].Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinitions)

