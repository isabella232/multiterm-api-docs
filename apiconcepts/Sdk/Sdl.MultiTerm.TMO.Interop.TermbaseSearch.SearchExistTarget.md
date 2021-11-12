#  SearchExistTarget property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SearchExistTarget —          Sets/returns whether only terms with one or more target terms should be taken into consideration.

## Type
Boolean
(read / write)

## Index Parameters
*none*

## Description

Set this property to true if you want the hit list to only contain terms with at least one corresponding target term. This property basically acts like a filter that singles out entries that have one or more target terms. The default value is false, i.e. usually also hit terms without a target term are taken into account.

## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.SearchExistTarget=true;
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```

