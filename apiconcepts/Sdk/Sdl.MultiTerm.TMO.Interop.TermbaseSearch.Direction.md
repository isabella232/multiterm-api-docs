# Direction property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Direction —          Sets/returns the search direction.

## Type
[Sdl.MultiTerm.TMO.Interop.MtSearchDirection](Sdl.MultiTerm.TMO.Interop.MtSearchDirection.md)
(read / write)

## Index Parameters
*none*

## Description

The search direction can be either up or down. The search direction value will usually be 'down', as a search is normally carried out from the start to and end of an index.

## Sample

```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```
