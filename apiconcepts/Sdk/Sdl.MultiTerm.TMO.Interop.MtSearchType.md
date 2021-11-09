

# 
    Sdl.MultiTerm.TMO.Interop.MtSearchType Enumeration



## Name

Sdl.MultiTerm.TMO.Interop.MtSearchType —          This enumerator contains the search types you can apply to a multiple termbase search.



## Description



When cascading a search over more than one termbase, you can set choose among three options:



## Values

* *mtHierarchial*

    You can either configure the search to stop as soon as hits have been found in a termbase. E.g. when the search has yielded a result in the first termbase, the other termbases are not searched. As only one termbase is searched in this case, the search will be carried out faster. This is the default option.
* *mtParallel*

    Choose this option to 'enforce' a lookup in all termbases, but have the results listed in alphabetical order regardless of the termbase name they come from.
* *mtSequential*

    Select this option to 'enforce' a lookup in all termbases and have the results listed per termbase.




## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MtSearchType)

