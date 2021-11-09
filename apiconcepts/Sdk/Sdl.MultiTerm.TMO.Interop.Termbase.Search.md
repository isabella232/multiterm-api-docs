

# 
    Search property



## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Search —          Provides programmatic access to the search functionality for a particular termbase.



## Type

[Sdl.MultiTerm.TMO.Interop.TermbaseSearch](Sdl.MultiTerm.TMO.Interop.TermbaseSearch.html)

(read)



## Index Parameters
*none*


## Description



Searching a termbase involves looking up a search expression in a selected index (i.e. the source index). By applying the Search property to a termbase you can create a search object, which you can then configure and execute to retrieve the search term from the source index.



## Sample


```cs
Termbase oTb = oTbs[0];
TermbaseSearch oSearch = oTb.Search;

//configure search operation
oSearch.MaximumHits=25;
oSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.SearchExpression="starship";
oSearch.SourceIndex="English";
oSearch.FuzzySearch=true;

HitTerms oHits = oSearch.Execute;
Debug.Write("Number of hits: " + oHits.Count);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.Search)

