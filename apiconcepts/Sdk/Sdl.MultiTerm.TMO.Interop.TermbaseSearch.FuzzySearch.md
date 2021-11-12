# FuzzySearch property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.FuzzySearch —          Sets/returns whether the termbase search should be a fuzzy search.

## Type
Boolean
(read / write)

## Index Parameters
*none*

## Description

Set this property to true, if you want to do a fuzzy search. The default value if false, i.e. by default no fuzzy search is performed.

Note: You could also put a hash sign '#' in front of the search expression to trigger a fuzzy search. This is a legacy from the old MultiTerm 5, in which a hash sign was used to indicate whether a search operation should be carried out as a fuzzy search.

## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.FuzzySearch=true;
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```

