

# 
    Sdl.MultiTerm.TMO.Interop.IndexesPermissions class



## Name

Sdl.MultiTerm.TMO.Interop.IndexesPermissions —          Provides programmatic access to the index permissions of the currently logged-in user.



## Description



Via this class you can retrieve information on the indexes (i.e. languages) the currently logged-in user has access to. You can use it, for example, to generate a list of indexes that the user can access. Note that this list is not necessarily identical to the list of indexes specified in the termbase definition, as certain users may not be allowed to see particular indexes in the first place.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.Count.html): Returns the number of indexes that the currently logged-in user can access.
* [Item](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.Item.html): Refers to a particular index permission.
* [ReadIndexes](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.ReadIndexes.html): Returns all indexes that the currently logged-in user has read-access too.
* [WriteIndexes](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.WriteIndexes.html): Returns all indexes the currently logged-in user has write access to.




## Methods
*None*


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

IndexesPermissions oIndexes = oTb.AccessPermissions.IndexesPermissions;
Debug.WriteLine("Number of indexes user can access: " + oIndexes.Count.ToString());

//list indexes
for(int i=0;i<oIndexes.Count;i++)
{
   	Debug.WriteLine(oIndexes[i].Label);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IndexesPermissions)

