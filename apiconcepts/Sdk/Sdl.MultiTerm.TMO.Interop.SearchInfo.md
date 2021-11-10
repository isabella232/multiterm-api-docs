

# 
    Sdl.MultiTerm.TMO.Interop.SearchInfo class




## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo —          Stores information on the search carried for particular termbases.



## Description



After a search has been carried out in multiple termbases you might want to know whether a particular termbases yielded any results, which source/target index has actually been used, etc. This class allows you to retrieve such information for each termbases included in the search.



## Properties
.md)
* [ErrorCode](Sdl.MultiTerm.TMO.Interop.SearchInfo.ErrorCode.md): Returns the error code for the search in a particular termbase (if applicable).
* [ErrorMessage](Sdl.MultiTerm.TMO.Interop.SearchInfo.ErrorMessage.md): Returns the error message for a search in a particular termbase (if applicable).
* [HitsFound](Sdl.MultiTerm.TMO.Interop.SearchInfo.HitsFound.md): Returns true or false depending on whether any hits have been found in a particular termbase.
* [SourceIndex](Sdl.MultiTerm.TMO.Interop.SearchInfo.SourceIndex.md): Returns the source index that was actually used when searching a particular termbase.
* [SourceLocale](Sdl.MultiTerm.TMO.Interop.SearchInfo.SourceLocale.md): Returns the locale of the source index used when searching a particular termbase.
* [TargetIndex](Sdl.MultiTerm.TMO.Interop.SearchInfo.TargetIndex.md): Returns the target index used when searching a particular termbase.
* [TargetLocale](Sdl.MultiTerm.TMO.Interop.SearchInfo.TargetLocale.md): Returns the locale of the target index used when searching a particular termbase.
* [TermbaseName](Sdl.MultiTerm.TMO.Interop.SearchInfo.TermbaseName.md): Returns the name of the termbase that the search info relates to.




## Methods
*None*


## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb1 = oTbs["Termbase1"];
Termbase oTb2 = oTbs["Termbase2"];
Termbase oTb3 = oTbs["Termbase3"];

MultiSearch oSearch = oMt.MultiSearch;
oSearch.SearchType = Sdl.MultiTerm.TMO.Interop.MtSearchType.mtSequential;
oSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
//guess the search index based on the index of the first termbase
oSearch.GuessIndex=Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.mtGuessIndex;
//maximum hits per termbase
oSearch.MaximumHits=10;
//add termbases to search
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");

oSearch.SearchExpression = "search term";

//execute search
HitTerms oHits = oSearch.Execute();

//retrieve information on search in the second termbase
SearchInfo oInfo;
oInfo = oSearch.SearchInfo[1];
Debug.WriteLine("Any hits found in this termbase? " + oInfo.HitsFound);
Debug.WriteLine("Source index used: " + oInfo.SourceIndex);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.SearchInfo)

