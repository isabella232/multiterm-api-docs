# Termbase property

## Name

Sdl.MultiTerm.TMO.Interop.HitTerm.Termbase —          Returns the name of the termbase in which a hit term was found.

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

Entries oEntries = oTb.Entries;

for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];				
   	Debug.WriteLine(oHit.Termbase);
}
```
