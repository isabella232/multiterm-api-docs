

# 
    MaximumHits property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.MaximumHits —          Sets/returns the maximum hit number.



## Type

Long

(read / write)



## Index Parameters
*none*


## Description



This property is used to limit the amount of hit terms returned by a search operation. If, for example, there are 10 matching entries in the termbase, but this property has been set to 5, only the first 5 hits will be returned.



## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.MaximumHits=10;
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="window";
tbSearch.SourceIndex="English";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.MaximumHits)

