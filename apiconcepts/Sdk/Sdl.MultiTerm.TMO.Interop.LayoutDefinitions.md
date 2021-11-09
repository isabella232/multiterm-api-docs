

# 
    Sdl.MultiTerm.TMO.Interop.LayoutDefinitions class



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinitions —          Provides programmatic access to the layout definitions of a termbase.



## Description



Via this class you can access the layout definitions associated with a particular termbase. You can use it to, for example, generate a list of available layouts.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Count.html): Returns the number of available layout definitions.
* [Item](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Item.html): Provides access to a particular layout definition.




## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Add.html): Adds a new layout definition to the collection.
* [Refresh](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Refresh.html): Updates the layout definition collection.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.StartWizard.html): Starts the Layout Definition wizard.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
Debug.Write("Number of layouts: +" + oLayouts.Count);

for(int i=0;i<oLayouts.Count;i++)
{
   	Debug.WritoLayouts[i].Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinitions)

