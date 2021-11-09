

# 
    AddSearchTermbase method



## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.AddSearchTermbase —          Adds a termbase to the MultiSearch.



## Returntype

void



## Parameters

* pxo\_termbase ([Sdl.MultiTerm.TMO.Interop.Termbase](Sdl.MultiTerm.TMO.Interop.Termbase.html))
* bstr\_source (String)
* bstr\_target (String)




## Description



This method is used to add termbases to a multiple termbase search. It requires a termbase object as well as the source and target index for each termbase as parameters. Note that if you use [GuessIndex](Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex.html) the search behaves as follows:

Suppose the source index for the first termbase is 'English'. In this case, the search in the second termbase will be carried out in the index that is 'guessed' to be the equivalent of the 'English' index in the first termbase, e.g. 'Englisch', 'ENG', etc. regardless of the source index that was provided as parameter for the second termbase. The same also applies to the target index.

Note: It is recommended that you add the termbases AFTER configuring all the other settings, e.g. after setting the [GuessIndex](Sdl.MultiTerm.TMO.Interop.MultiSearch.GuessIndex.html) property.



## Sample


```cs
//select termbases
Termbase oTb1 = oTbs["Termbase1"];
Termbase oTb2 = oTbs["Termbase2"];
Termbase oTb3 = oTbs["Termbase3"];

//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;
//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "");
oSearch.AddSearchTermbase(oTb2, "Deutsch", "Englisch");
oSearch.AddSearchTermbase(oTb3, "DEU", "ENG");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MultiSearch.AddSearchTermbase)

