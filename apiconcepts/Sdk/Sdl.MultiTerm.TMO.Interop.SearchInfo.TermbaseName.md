#  TermbaseName property

## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo.TermbaseName —          Returns the name of the termbase that the search info relates to.

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
Debug.WriteLine("Target name: " + oInfo.TermbaseName);
```
