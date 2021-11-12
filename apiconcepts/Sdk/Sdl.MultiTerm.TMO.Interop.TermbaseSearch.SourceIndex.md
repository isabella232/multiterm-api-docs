#   SourceIndex property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SourceIndex —          Sets/returns the search index.

## Type
String
(read / write)

## Index Parameters
*none*

## Description


A termbase search is carried out in a particular index. Via this property you can determine the index (language) in which the search should be performed, e.g. 'English'.


## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.SourceIndex="English";
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;
```

