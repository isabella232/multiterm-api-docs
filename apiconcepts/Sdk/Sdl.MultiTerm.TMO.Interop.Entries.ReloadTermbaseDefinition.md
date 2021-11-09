

# 
    ReloadTermbaseDefinition method



## Name

Sdl.MultiTerm.TMO.Interop.Entries.ReloadTermbaseDefinition —          Refreshes the current termbase definition.



## Returntype

void



## Parameters
*none*


## Description



By applying this method you can make sure that you are always using the most up-to-date termbase definition, e.g. when the termbase definition is edited while using the termbase.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

oEntries.ReloadTermbaseDefinition();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Entries.ReloadTermbaseDefinition)

