

# 
    CancelSearch method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.CancelSearch —          Cancels the search operation.



## Returntype

void



## Parameters
*none*


## Description





## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.SourceIndex="English";			
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.MaximumHits=10;

tbSearch.CancelSearch();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.CancelSearch)

