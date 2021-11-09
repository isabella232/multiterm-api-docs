

# 
    SearchExpression property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SearchExpression —          Sets/returns the search expression.



## Type

String

(read / write)



## Index Parameters
*none*


## Description



This property sets the search terms used for a search operation. If this parameter is left unspecified, a blank string ("") will be used, which means that any term will be retrieved from the termbase.

Note: MultiTerm allows to use the asterisk (\*) as a placeholder in search operations. Moreover, you can also carry out a character range search. To search for terms within a specific character ranges, use square brackets, e.g. "[a-b]".



## Sample


```cs
TermbaseSearch tbSearch = oTb.Search;

tbSearch.SearchExpression="window";
tbSearch.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
tbSearch.MaximumHits=10;
tbSearch.SourceIndex="English";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseSearch.SearchExpression)

