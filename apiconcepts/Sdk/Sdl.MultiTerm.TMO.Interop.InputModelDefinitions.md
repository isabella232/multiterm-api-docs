

# 
    Sdl.MultiTerm.TMO.Interop.InputModelDefinitions class



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinitions —          Provides programmatic access to the input model definitions of a termbase.



## Description



Via this class you can access the input model definitions associated with a particular termbase. You can use it to, for example, generate a list of available input models.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Count.html): Returns the number of available input model definitions.
* [Item](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Item.html): Provides access to a particular input model definition.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Add.html): Adds a new input model definition to the collection.
* [Refresh](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Refresh.html): Updates the input model definition collection.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.StartWizard.html): Starts the Input Model Definition wizard.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oModels = oTb.InputModelDefinitions;
Debug.Write("Number of input models: +" + oModels.Count);

for(int i=0;i<oModels.Count;i++)
{
   	Debug.Write(oModels[i].Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinitions)

