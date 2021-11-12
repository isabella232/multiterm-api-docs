# ClearSearchTermbases method

## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.ClearSearchTermbases —          Removes all termbases from the MultiSearch.

## Returntype

void

## Parameters
*none*

## Description

You can apply this property, for example, to make sure that no termbases are associated with the MultiSearch before adding other termbases.

It is recommended to apply this method before adding termbases to a multi search, also to make sure that any source/target language changes are taken over correctly.

## Sample


```cs
//create MultiSearch object
MultiSearch oSearch = oMt.MultiSearch;

//remove any termbases associated with the MultiSearch first
oSearch.ClearSearchTermbases();

//add termbases to multisearch
oSearch.AddSearchTermbase(oTb1, "English", "");
oSearch.AddSearchTermbase(oTb2, "Deutsch", "Englisch");
oSearch.AddSearchTermbase(oTb3, "DEU", "ENG");
```

