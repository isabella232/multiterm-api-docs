

# 
    Sdl.MultiTerm.TMO.Interop.Indexes class




## Name

Sdl.MultiTerm.TMO.Interop.Indexes —          Provides programmatic access to a particular index in the termbase definition.



## Description



This class provides programmatic access to a specific index (i.e. language) contained in a termbase definition. You can use this class, for example, to generate a list of all languages contained in the definition of a particular termbase.
.md)
Note that this class gives access to all languages contained in the termbase definition, not only to the languages that a user can access. If you want to generate a list that contains only the languages the currently logged-in user has access to, you should rather use the [IndexesPermissions](Sdl.MultiTerm.TMO.Interop.IndexesPermissions.md) class.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.Indexes.Count.md): Returns the number of indexes (i.e. languages) contained in a termbase definition.
* [Item](Sdl.MultiTerm.TMO.Interop.Indexes.Item.md): Provides access to a specific termbase index.




## Methods
*None*


## Sample


```cs
TermbaseDefinition tbDef = oTb.Definition;
Indexes oIndexes = tbDef.Indexes;
Debug.Write("Number of languages: " + oIndexes.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Indexes)

