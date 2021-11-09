

# 
    StartingEntryID property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.StartingEntryID —          Sets/returns the entry id from which the search should be started.



## Type

Long

(read / write)



## Index Parameters
*none*


## Description



Suppose you would like the termbase search to start from the entry with the id '100'. In this case, set this property to the value 100.



## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.StartingEntryID=100;
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.SearchExpression="Abla�schraube";
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.StartingEntryID)

