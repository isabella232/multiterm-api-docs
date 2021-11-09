

# 
    FuzzySearch property



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.FuzzySearch —          Turns on/off fuzzy search.



## Type

Boolean

(read / write)



## Index Parameters
*none*


## Description



By setting this property to 'true', a fuzzy search will be performed in the termbase(s). The default value if 'false'.

Setting this property to any value will automatically set FullTextSearch to 'false' and vice versa.



## Sample


```cs
//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//define search properties
oSearch.FuzzySearch=true;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SearchExpression="window";

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.FuzzySearch)

