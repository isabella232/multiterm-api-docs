#  TargetRequired property

## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.TargetRequired —          Sets/returns whether only terms with one or more target terms should be taken into consideration.

## Type

Boolean
(read / write)

## Index Parameters
*none*

## Description


Set this property to true if you want the hit list to only contain terms with at least one corresponding target term. This property basically acts like a filter that singles out entries that have one or more target terms. The default value is false, i.e. usually also hit terms without a target term are taken into account.

## Sample


```cs
//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//define search properties
oSearch.TargetRequired=true;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SearchExpression="window";
oSearch.FuzzySearch=true;

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");
```
