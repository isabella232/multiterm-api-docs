# SearchScore property

## Name

Sdl.MultiTerm.TMO.Interop.HitTerm.SearchScore —          Returns the fuzziness score for a particular hit term.

## Type

Long
(read)

## Index Parameters
*none*

## Description

The fuzzy search allows MultiTerm to find the closest approximation to a search expression. Via this property you can ascertain how closely a hit term resembles the actual search expression. You can use this information, for example, in order not to display hit terms that are below a certain fuzziness percentage.



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

//only display matches greater than 80%
for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];				
   	if(oHit.SearchScore > 80)
   	{
      		Debug.WriteLine(oHit.Text);
   	}
}
```
