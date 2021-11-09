

# 
    Refresh method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Refresh —          Updates the termbase information.



## Returntype

void



## Parameters
*none*


## Description



This method is useful to make sure that the user always sees the most up-to-date termbase information, e.g. to make any additions to the termbase reflect in the total termbase entry count.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
tbInfo.Refresh();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Refresh)

