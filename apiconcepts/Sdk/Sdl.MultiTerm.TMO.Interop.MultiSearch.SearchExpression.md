

# 
    SearchExpression property



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchExpression —          Sets/returns the expression to look up.



## Type

String

(read / write)



## Index Parameters
*none*


## Description



Via this property you provide the search term to look up in the termbase(s).  If this parameter is left unspecified, a blank string ("") will be used, which means that any term will be retrieved from the termbase.

Note: MultiTerm allows to use the asterisk (\*) as a placeholder in search operations. Moreover, you can also carry out a character range search. To search for terms within a specific character ranges, use square brackets, e.g. "[a-b]".



## Sample


```cs
//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//define search properties
oSearch.SearchExpression="star system";
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.FuzzySearch=true;

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.SearchExpression)

