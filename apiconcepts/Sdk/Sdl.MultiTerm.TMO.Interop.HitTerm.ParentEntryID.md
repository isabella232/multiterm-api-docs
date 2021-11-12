# ParentEntryID property
## Name

Sdl.MultiTerm.TMO.Interop.HitTerm.ParentEntryID —          Returns the entry id associated with a particular hit term.

## Type

String
(read)

## Index Parameters
*none*

## Description

Suppose you would like to implement a function that allows users to click a hit term in the list to display the entire entry content, i.e. copy the functionality provided in MultiTerm Workstation. Each entry is uniquely identified via its entry id. This is why the HitTerm class allows you to retrieve the id of the entry the hit term belongs to.

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
Entry oEntry;
for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];				
   	int myId = Convert.ToInt32(oHit.ParentEntryID);
   	oEntry = oEntries.Item(myId);
   	Debug.WriteLine(oEntry.Content.Content);
}
```
