

# 
    Information property



## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Information —          Provides programmatic access to the termbase information.



## Type

[Sdl.MultiTerm.TMO.Interop.TermbaseInformation](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.html)

(read)



## Index Parameters
*none*


## Description



Applying this property to a termbase object allows you to retrieve various information on the specified termbase such as the termbase creation date, the total number of entries, the physical size of the termbase, the full termbase name, which includes the termbase name as well as the location (i.e. name of the machine on which it is hosted), etc.



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

TermbaseInformation oInfo = oTb.Information;

Debug.Write("Termbase creation date: " + oInfo.CreationDate);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.Information)

