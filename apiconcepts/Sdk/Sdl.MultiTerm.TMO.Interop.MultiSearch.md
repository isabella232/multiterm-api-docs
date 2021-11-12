# Sdl.MultiTerm.TMO.Interop.MultiSearch class

## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch —          Provides programmatic access to multiple termbase search.

## Description

Rather than searching only in a single termbase, MultiTerm allows you to cascade searches over sevral termbases, which can both be local and remote server termbases. This is why the MultiSearch class is sub-ordinate to the MultiTerm client application class, as it is not limited to the local or server termbase repository.

You can avail of this class to implement multiple termbase search functionality in your client application. Rather than carrying out a search on each termbase, you can add multiple termbases to one MultiSearch object, execute the search and then retrieve a consolidated hit list for all termbases.

A search requires you to specify the search index for each termbase. Multiple termbase search can be tricky, if the search index label differs among the various termbases.  Example: you would like to carry out a search for an English term in three termbases. Termbase#1 has an index called "English", Termbase#2 has an index called "Englisch", and Termbase#3 has an index called "ENG".

To carry out a search in the English index of all three termbases you would have to find out which index label stands for the English language in each termbase.
The MultiSearch class implements a [GuessIndex](Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex.md) property that allows you to have the search 'guess' the correct index. If, for example,  the first termbase you add to the search has the index label "English", the search will automatically 'guess' what the English index is called in all the other termbases. As a criterion for 'guessing' the correct search index, the MultiSearch relies on the index locales.

In the example below the second termbases added to the search in "Deutsch" (i.e. German). However, the search is configured to 'guess' the index, i.e. in the second and third termbase the search will be carried out in the indexes that are most likely to correspond to the "English" index of the first termbase.

## Properties

* [Direction](Sdl.MultiTerm.TMO.Interop.MultiSearch.Direction.md): Sets/returns the direction for the multiple termbase search.
* [FuzzySearch](Sdl.MultiTerm.TMO.Interop.MultiSearch.FuzzySearch.md): Turns on/off fuzzy search. Setting this property to any value will automatically set FullTextSearch to 'false'
* [FullTextSearch](Sdl.MultiTerm.TMO.Interop.MultiSearch.FullTextSearch.md): Turns on/off full text search. Setting this property to any value will automatically set FuzzySearch to 'false'
* [GuessIndex](Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex.md): Specifies whether the index for the multiple termbase search should be guessed or not.
* [MaximumHits](Sdl.MultiTerm.TMO.Interop.MultiSearch.MaximumHits.md): Sets/returns the maximum number of hits per termbase.
* [SearchExpression](Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchExpression.md): Sets/returns the expression to look up.
* [SearchInfo](Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchInfo.md): Provides programmatic access to the search information related to a particular termbase.
* [SearchTermbases](Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchTermbases.md): Returns the names of the termbases used for a multi search in an XML stream.
* [SearchType](Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchType.md): Specifies the type of multiple termbase search to carry out.
* [TargetRequired](Sdl.MultiTerm.TMO.Interop.MultiSearch.TargetRequired.md): Sets/returns whether only terms with one or more target terms should be taken into consideration.


## Methods

* [AddSearchTermbase](Sdl.MultiTerm.TMO.Interop.MultiSearch.AddSearchTermbase.md): Adds a termbase to the MultiSearch.
* [ClearSearchTermbases](Sdl.MultiTerm.TMO.Interop.MultiSearch.ClearSearchTermbases.md): Removes all termbases from the MultiSearch.
* [Execute](Sdl.MultiTerm.TMO.Interop.MultiSearch.Execute.md): Executes the MultiSearch operation and stores the results in a HitTerms object.


## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;

//select termbases
Termbase oTb1 = oTbs["C:\\TestData\\Termbase1"];
Termbase oTb2 = oTbs["C:\\TestData\\Termbase2"];
Termbase oTb3 = oTbs["C:\\TestData\\Termbase3"];

//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//define further search properties
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SearchExpression="window";
oSearch.GuessIndex=Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.mtGuessIndex;
oSearch.SearchType=Sdl.MultiTerm.TMO.Interop.MtSearchType.mtParallel;

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");

//execute search and output hitterms
HitTerms oHits = oSearch.Execute();
for(int i=0;i<oHits.Count;i++)
{
  	Debug.WriteLine(oHits[i].Text);
  	Debug.WriteLine(oHits[i].Termbase);
}
```

