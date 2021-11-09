

# 
    SearchType property



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchType —          Specifies the type of multiple termbase search to carry out.



## Type

[Sdl.MultiTerm.TMO.Interop.MtSearchType](Sdl.MultiTerm.TMO.Interop.MtSearchType.html)

(read / write)



## Index Parameters
*none*


## Description





## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb1 = oTbs["Termbase1"];
Termbase oTb2 = oTbs["Termbase2"];
Termbase oTb3 = oTbs["Termbase3"];

MultiSearch oSearch = oMt.MultiSearch;
oSearch.SearchType = Sdl.MultiTerm.TMO.Interop.MtSearchType.mtParallel;
oSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
//guess the search index based on the index of the first termbase
oSearch.GuessIndex=Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.mtGuessIndex;
//maximum hits per termbase
oSearch.MaximumHits=10;

//add termbases to search
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchType)

