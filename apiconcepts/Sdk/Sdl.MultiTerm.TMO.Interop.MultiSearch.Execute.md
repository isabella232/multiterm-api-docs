

# 
    Execute method



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.Execute —          Executes the MultiSearch operation and stores the results in a HitTerms object.



## Returntype

[Sdl.MultiTerm.TMO.Interop.HitTerms](Sdl.MultiTerm.TMO.Interop.HitTerms.html)



## Parameters
*none*


## Description



By applying the Execute method to a MultiSearch,  the search is carried out in all termbases. This method is also used to create a HitTerms object, from which the search results (hit terms) can be retrieved.



## Sample


```cs
//select termbases
Termbase oTb1 = oTbs["Termbase1"];
Termbase oTb2 = oTbs["Termbase2"];
Termbase oTb3 = oTbs["Termbase3"];

//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;


//define search properties
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SearchExpression="window";
oSearch.FuzzySearch=true;
oSearch.GuessIndex=Sdl.MultiTerm.TMO.Interop.MtIndexGuessing.mtGuessIndex;

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "");
oSearch.AddSearchTermbase(oTb2, "Englisch", "Deutsch");
oSearch.AddSearchTermbase(oTb3, "ENG", "DEU");

//execute search and output hitterms
HitTerms oHits = oSearch.Execute();
for(int i=0;i<oHits.Count;i++)
{
   	Debug.WriteLine(oHits[i].Text);
   	Debug.WriteLine(oHits[i].Termbase);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.Execute)

