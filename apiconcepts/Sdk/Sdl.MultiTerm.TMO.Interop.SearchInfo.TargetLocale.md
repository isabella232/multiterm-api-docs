# TargetLocale property

## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo.TargetLocale —          Returns the locale of the target index used when searching a particular termbase.

## Type

String
(read)

## Index Parameters
*none*


## Description


## Sample


```cs
//execute search
HitTerms oHits = oSearch.Execute();

//retrieve information on search in the second termbase
SearchInfo oInfo;
oInfo = oSearch.SearchInfo[1];
Debug.WriteLine("Target locale: " + oInfo.TargetLocale);
```