

# 
    LastTerm property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.LastTerm —          Sets the last term from which a search operation should be started.



## Type

String

(write)



## Index Parameters
*none*


## Description



Suppose you would like to search for the term 'window'. Afterwards you would like to search for all terms beginning with window that come after the term 'window' itself. In this case you can use this property to set 'window' as the last term from which the search should be started.



## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.LastTerm = "window";
tbSearch.SearchExpression="window*";
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.LastTerm)

