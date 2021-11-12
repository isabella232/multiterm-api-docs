#  TargetIndex property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.TargetIndex —          Sets/returns the search target index.


## Type
String
(read / write)

## Index Parameters
*none*

## Description

This property can be used to set the target index for a search operation. This parameter is optional, it only plays a role when the SearchExistTarget property is set to true. To retrieve the target term for a (source) hit term, you need to go inside the XML stream of the entry content and retrieve the target index from there.

## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.TargetIndex ="German";
tbSearch.SourceIndex="English";			
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;
```
