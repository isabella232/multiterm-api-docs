

# 
    Reorganise method



## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Reorganise —          Reorganises a specified termbase.



## Returntype

void



## Parameters
*none*


## Description



To ensure optimum termbase performance termbases need to be reorganised from time to time. During a termbase reorganisation the fuzzy index is updated. The fuzzy index is created automatically by MultiTerm. It makes sure that the best approximation to your search expression is found, even if the search term is misspelled.

Termbases are reorganised by default every time you import data. However, you should reorganise your termbase data on a regular basis whether you are carrying out imports or not.

Local termbases can be reorganised by the respective user. Server termbases need to be reorganised by the termbase administrator, since exclusive access is required for this operation.

A termbase is reorganised by applying the Reorganise method to the corresponding Termbase object.



## Sample


```cs
Termbase oTb = oTbs[0];
oTb.Reorganise();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.Reorganise)

