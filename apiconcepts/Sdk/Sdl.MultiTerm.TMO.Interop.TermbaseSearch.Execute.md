

# 
    Execute method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Execute —          Executes a search operation and stores the results in a HitTerms object.



## Returntype

[Sdl.MultiTerm.TMO.Interop.HitTerms](Sdl.MultiTerm.TMO.Interop.HitTerms.html)



## Parameters
*none*


## Description



By applying the Execute method to a termbase search object, the search is actually carried out. This method is also used to create a HitTerms object, from which the search results (hit terms) can be retrieved.

You have to specify at least the source index and the search expression.



## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.SourceIndex="English";			
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="Abla�schraube";
tbSearch.MaximumHits=10;

HitTerms oHits = tbSearch.Execute();
Debug.Write("Number of hits found: " + oHits.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.Execute)

