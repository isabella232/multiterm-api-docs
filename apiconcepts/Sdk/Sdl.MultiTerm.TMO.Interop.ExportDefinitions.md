# Sdl.MultiTerm.TMO.Interop.ExportDefinitions class


## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinitions —          Provides programmatic access to the export definitions of a termbase.



## Description



Via this class you can access the export definitions associated with a particular termbase. You can use it to, for example, generate a list of available export definitions.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Count.md): Returns the number of available export definitions.
* [Item](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Item.md): Provides access to a particular export definition.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Add.md): Adds a new export definition to the collection.
* [Refresh](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Refresh.md): Updates the export definition collection.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.ExportDefinitions.StartWizard.md): Starts the Export Definition wizard.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;
Debug.Write("Number of export definitions: +" + oExpDefs.Count);

for(int i=0;i<oExpDefs.Count;i++)
{
   	Debug.Write(oExpDefs[i].Name);
}
```


