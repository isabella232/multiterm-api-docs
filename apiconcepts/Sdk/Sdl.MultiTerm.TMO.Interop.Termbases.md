# Sdl.MultiTerm.TMO.Interop.Termbases class

## Name

Sdl.MultiTerm.TMO.Interop.Termbases —          Provides programmatic access to a termbase collection.

## Description

This class allows you to retrieve all termbases of your local termbase repository or the termbases from the server repository that you are allowed to gain access to with your login. You can use this class to, for example, generate a list of all termbases available in a particular repository.

## Properties
* [Count](Sdl.MultiTerm.TMO.Interop.Termbases.Count.md): Returns the number of available termbases.
* [Item](Sdl.MultiTerm.TMO.Interop.Termbases.Item.md): Provides programmatic access to a specific termbase.

## Methods

* [Add](Sdl.MultiTerm.TMO.Interop.Termbases.Add.md): Allows you to add existing file based termbases to the local repository programmatically.
* [New](Sdl.MultiTerm.TMO.Interop.Termbases.New.md): Creates a new termbase programmatically.
* [Refresh](Sdl.MultiTerm.TMO.Interop.Termbases.Refresh.md): Refreshes a termbase collection.
* [Remove](Sdl.MultiTerm.TMO.Interop.Termbases.Remove.md): Removes a termbase from a local termbase collection.


## Sample


```cs
Termbases oTbs = oServRep.Termbases;

for(int i=0;i<oTbs.Count;i++)
{
   	Debug.WriteLine("Termbase name: " + oTbs[i].Name);
}
```
