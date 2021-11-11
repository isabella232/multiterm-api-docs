# Sdl.MultiTerm.TMO.Interop.HitTerms class




## Name

Sdl.MultiTerm.TMO.Interop.HitTerms —          Provides programmatic access to the results of a search or browse operation.



## Description


When executing a [search](Sdl.MultiTerm.TMO.Interop.Termbase.Browse.md) or [browse](Sdl.MultiTerm.TMO.Interop.Termbase.Search.md) operation the results need to be stored in a HitTerms object, from which they can then be retrieved.

You can use the HitTerms object to return the number of hits found (if any) and to loop through them.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.HitTerms.Count.md): Returns the number of hit terms found.
* [Item](Sdl.MultiTerm.TMO.Interop.HitTerms.Item.md): Refers to a particular hit term.




## Methods
*None*


## Sample


```cs
//example of browse operation
Termbase oTb = oTbs["Termbase name"];
TermbaseBrowser oBrowser = oTb.Browse;
oBrowser.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
oBrowser.MaximumTermCount = 1;
oBrowser.StartTerm="";
oBrowser.SourceIndex="English";

HitTerms oHits = oBrowser.Execute();
Debug.Write(oHits[0].Text);

//example of search operation
Termbase oTb = oTbs["Termbase name"];
TermbaseSearch oSearch = oTb.Search;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SourceIndex="English";
oSearch.SearchExpression ="starship";

HitTerms oHits = oSearch.Execute();
for(int i=0;i<oHits.Count;i++)
{
   	Debug.WriteLine(oHits[i].Text);
}
```


