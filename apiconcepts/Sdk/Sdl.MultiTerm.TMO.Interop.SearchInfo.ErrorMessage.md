# ErrorMessage property

## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo.ErrorMessage —          Returns the error message for a search in a particular termbase (if applicable).

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
Debug.WriteLine("Error message " + oInfo.ErrorMessage);
```