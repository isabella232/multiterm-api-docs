

# 
    Sdl.MultiTerm.TMO.Interop.Index class



## Name

Sdl.MultiTerm.TMO.Interop.Index —          Provides programmatic access to a particular index of a termbase definition.



## Description



This class allows you to retrieve, for example, the corresponding index label, the locale, etc.



## Properties

* [Fields](Sdl.MultiTerm.TMO.Interop.Index.Fields.html): Provides programmatic access to the entry-level descriptive fields.
* [Label](Sdl.MultiTerm.TMO.Interop.Index.Label.html): Returns the label of a particular index.
* [Language](Sdl.MultiTerm.TMO.Interop.Index.Language.html): Returns the name of the index language.
* [Locale](Sdl.MultiTerm.TMO.Interop.Index.Locale.html): Returns the locale of the index.
* [TargetOnly](Sdl.MultiTerm.TMO.Interop.Index.TargetOnly.html): Flags whether the current index can be used only as target index.
* [TermFields](Sdl.MultiTerm.TMO.Interop.Index.TermFields.html): Provides programmatic access to the term-level descriptive fields.




## Methods
*None*


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition oDef = oTb.Definition;
Indexes oIndexes = oDef.Indexes;

//select first index
Index oIndex = oIndexes[0];
Debug.WriteLine(oIndex.Label);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Index)

