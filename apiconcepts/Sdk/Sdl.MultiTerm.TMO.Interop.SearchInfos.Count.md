#  Count property

## Name

Sdl.MultiTerm.TMO.Interop.SearchInfos.Count —          Returns the number of search info sets available.

## Type

Long
(read)


## Index Parameters
*none*

## Description


Each search info set relates to a particular termbase. So, the value returned by this property will be equal to the number of termbases used during the search.

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
Debug.WriteLine("Number of search info sets available: " + infos.Count.ToString());
```
