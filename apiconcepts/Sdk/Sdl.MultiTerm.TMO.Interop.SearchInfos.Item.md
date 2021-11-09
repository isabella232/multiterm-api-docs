

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.SearchInfos.Item —          Refers to a particular set of search info, i.e. the search info related to a specific termbase.



## Type

[Sdl.MultiTerm.TMO.Interop.SearchInfo](Sdl.MultiTerm.TMO.Interop.SearchInfo.html)

(read)



## Index Parameters

* Index (Variant)




## Description



This property allows you, for example, to retrieve information such as the source/target index that was actually used when searching a particular termbase in a multi-termbase search.



## Sample


```cs
Sdl.MultiTerm.TMO.Interop.MultiSearch search = oMt.MultiSearch;
search.MaximumHits=10;
search.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
search.SearchExpression="";
search.AddSearchTermbase(oTermbase1, "English", "German");
search.AddSearchTermbase(oTermbase1, "ENG", "DEU");

search.Execute();

Sdl.MultiTerm.TMO.Interop.SearchInfos infos = search.SearchInfo;
Debug.WriteLine("Source index used for the first termbase: " + infos[0].SourceIndex);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.SearchInfos.Item)

