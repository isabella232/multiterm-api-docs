

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.HitTerms.Count —          Returns the number of hit terms found.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many hit terms have been found (if any) for a search or browse operation.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];
TermbaseSearch oSearch = oTb.Search;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SourceIndex="English";
oSearch.SearchExpression ="starship";

HitTerms oHits = oSearch.Execute();
if(oHits.Count==0)
{
   	Debug.WriteLine("No hits found");
} else {
   	Debug.WriteLine("Number of hits found: " + oHits.Count.ToString());
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.HitTerms.Count)

