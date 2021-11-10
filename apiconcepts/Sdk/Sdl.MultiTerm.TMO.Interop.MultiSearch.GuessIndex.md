

# 
    GuessIndex property




## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex —          Specifies whether the index for the multiple termbase search should be guessed or not.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.MtIndexGuessing](Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.md)

(read / write)



## Index Parameters
*none*


## Description



When performing a multiple termbase search you need to take into consideration that the search index used in the first termbase is named differently in the other termbases. For example, while the search index is called "English" in the first termbase, in the other termbases it may be called "Englisch", "ENG", etc.

By setting this parameter you can make the search 'guess' the search index based on the search index selected for the first termbase. In this case even when, for example, "Deutsch" has been specified for the second termbase, the search will still be carried out in the English index.

The determination is made by the search automatically based on the index locale.

Note: We recommend that you configure this setting BEFORE [adding the search termbases](Sdl.MultiTerm.TMO.Interop.MultiSearch.AddSearchTermbase.md).



## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb1 = oTbs["Termbase1"];
Termbase oTb2 = oTbs["Termbase2"];
Termbase oTb3 = oTbs["Termbase3"];

MultiSearch oSearch = oMt.MultiSearch;
//guess the search index based on the index of the first termbase
oSearch.GuessIndex=Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.mtGuessIndex;

oSearch.SearchType = Sdl.MultiTerm.TMO.Interop.MtSearchType.mtSequential;
oSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
//maximum hits per termbase
oSearch.MaximumHits=10;

//add termbases to search
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");
oSearch.SearchExpression = "language";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex)

