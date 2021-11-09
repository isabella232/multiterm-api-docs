

# 
    ErrorCode property



## Name

Sdl.MultiTerm.TMO.Interop.SearchInfo.ErrorCode —          Returns the error code for the search in a particular termbase (if applicable).



## Type

Long

(read)



## Index Parameters
*none*


## Description





## Sample


```cs
//execute search
HitTerms oHits = oSearch.Execute();

//retrieve information on search in the second termbase
SearchInfo oInfo;
oInfo = oSearch.SearchInfo[1];
Debug.WriteLine("Error code " + oInfo.ErrorCode);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.SearchInfo.ErrorCode)

