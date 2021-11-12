# Index property

## Name

Sdl.MultiTerm.TMO.Interop.HitTerm.Index —          Returns the name of the index in which a hit term has been found.

## Type

String
(read)

## Index Parameters
*none*

## Description

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];
TermbaseSearch oSearch = oTb.Search;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SourceIndex="English";
oSearch.SearchExpression ="starship";

HitTerms oHits = oSearch.Execute();
HitTerm oHit;
for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];
   	Debug.WriteLine(oHit.Index);
}
```
