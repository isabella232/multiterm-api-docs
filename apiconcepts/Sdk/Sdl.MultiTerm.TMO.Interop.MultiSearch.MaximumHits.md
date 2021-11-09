

# 
    MaximumHits property



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.MaximumHits —          Sets/returns the maximum number of hits per termbase.



## Type

Long

(read / write)



## Index Parameters
*none*


## Description



Settings this property, e.g. to 10 will list up to ten hits for each termbase, even if one or several termbases potentially contain more hit terms.



## Sample


```cs
//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//define search properties
oSearch.MaximumHits=10;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.SearchExpression="window";
oSearch.FuzzySearch=true;

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "German");
oSearch.AddSearchTermbase(oTb2, "Deutsch", "Englisch");
oSearch.AddSearchTermbase(oTb3, "DEU", "ENG");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.MaximumHits)

