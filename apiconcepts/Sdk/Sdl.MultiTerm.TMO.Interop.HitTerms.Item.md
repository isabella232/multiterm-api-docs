

# 
    Item property




## Name

Sdl.MultiTerm.TMO.Interop.HitTerms.Item —          Refers to a particular hit term.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.HitTerm](Sdl.MultiTerm.TMO.Interop.HitTerm.md)

(read)



## Index Parameters

* Index (Variant)




## Description



This class allows you to retrieve a particular hit term from a hit terms collection, e.g. to output the actual hit term content, the associated entry id, etc.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];
TermbaseSearch oSearch = oTb.Search;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SourceIndex="English";
oSearch.SearchExpression ="starship";

HitTerms oHits = oSearch.Execute();
Debug.WriteLine(oHits[0].Text);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.HitTerms.Item)

