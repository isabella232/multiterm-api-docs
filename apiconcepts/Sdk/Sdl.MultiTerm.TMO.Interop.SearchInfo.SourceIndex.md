#  SourceIndex property

## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo.SourceIndex —          Returns the source index that was actually used when searching a particular termbase.

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
Debug.WriteLine("Source index used " + oInfo.SourceIndex);
```

