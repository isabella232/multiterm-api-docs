

# 
    Sdl.MultiTerm.TMO.Interop.ImportDefinitions class



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions —          Provides programmatic access to the import definitions of a termbase.



## Description



Via this class you can access the import definitions associated with a particular termbase. You can use it to, for example, generate a list of available import definitions.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Count.html): Returns the number of available import definitions.
* [Item](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Item.html): Provides access to a particular import definition.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Add.html): Adds a new import definition to the collection.
* [Refresh](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Refresh.html): Updates the import definition collection.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.ImportDefinitions.StartWizard.html): Starts the Import Definition wizard.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oImpDefs = oTb.ImportDefinitions;
Debug.Write("Number of import definitions: +" + oImpDefs.Count);

for(int i=0;i<oImpDefs.Count;i++)
{
   	Debug.WritoImpDefsfs[i].Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinitions)

