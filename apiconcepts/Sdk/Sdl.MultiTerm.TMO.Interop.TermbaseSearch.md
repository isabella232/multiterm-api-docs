# Sdl.MultiTerm.TMO.Interop.TermbaseSearch class




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch —          Provides programmatic access to the MultiTerm search functionality.



## Description



Searching a termbase involves retrieving one or more hit terms from the search index (i.e. the currently selected source index of a particular termbase). The search result yields terms from this index only.

The search expression can be a full term, e.g. "windows", it can be part of an existing term, e.g. "win", or it could be a search string with wildcards, e.g. "\*window\*".

MultiTerm also supports different types of search, such as an exact search to look up an exact search term and the so-called fuzzy search, which returns the best approximation(s) to a search term.

When doing a termbase search you need to provide various parameters such as the search term, the maximum number of hit terms, the search index, and the search direction (up or down). The result of a search needs to be stored in a HitTerms object. This object is created by applying the Execute method to the termbase search. From the HitTerms object you can then retrieve various information such as the number of hits found, the hit terms themselves, etc.



## Properties
* [Direction](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Direction.md): Sets/returns the search direction.
* [FuzzySearch](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.FuzzySearch.md): Sets/returns whether the termbase search should be a fuzzy search.
* [LastTerm](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.LastTerm.md): Sets the last term from which a search operation should be started.
* [MaximumHits](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.MaximumHits.md): Sets/returns the maximum hit number.
* [SearchExistTarget](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SearchExistTarget.md): Sets/returns whether only terms with one or more target terms should be taken into consideration.
* [SearchExpression](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SearchExpression.md): Sets/returns the search expression.
* [SourceIndex](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SourceIndex.md): Sets/returns the search index.
* [StartingEntryID](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.StartingEntryID.md): Sets/returns the entry id from which the search should be started.
* [TargetIndex](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.TargetIndex.md): Sets/returns the search target index.




## Methods

* [Advise](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Advise.md): [For internal use only.]
* [CancelSearch](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.CancelSearch.md): Cancels the search operation.
* [Execute](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Execute.md): Executes a search operation and stores the results in a HitTerms object.
* [Unadvise](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Unadvise.md): [For internal use only]




## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="a*";
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";

HitTerms oHits = tbSearch.Execute();
Debug.Write("Number of hits found: " + oHits.Count.ToString());
```

