#  StartSearch event

## Name

Sdl.MultiTerm.TMO.Interop.MultiSearch.StartSearch —          This event is triggered upon the start of a filtered search.


## Event handler

StartSearch(ByVal TotalEntriesForFilter as Long, ByVal CurrentTermbase as Long, ByVal TotalTermbases as Long)

## Description

You can use this event to provide information to the user upon starting a filtered search, i.e. the total number of termbases that need to be searched, the currently searched termbase, as well as the total number of entries to filter.
