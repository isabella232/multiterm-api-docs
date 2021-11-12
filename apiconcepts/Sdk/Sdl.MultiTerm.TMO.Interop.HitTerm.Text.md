# Text property

## Name

Sdl.MultiTerm.TMO.Interop.HitTerm.Text —          Returns the actual hit term.

## Type

String
(read)


## Index Parameters
*none*

## Description

This property is used to return the actual hit term content. This is probably the most frequently used property of the HitTerm class, as it is used to generate the hit term list.

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

//generate hit list
for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];				
   	Debug.WriteLine(oHit.Text);
}
```