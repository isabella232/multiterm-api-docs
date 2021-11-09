

# 
    IsReadOnly property



## Name

Sdl.MultiTerm.TMO.Interop.Termbase.IsReadOnly —          Returns True or False depending on whether a termbase is read-only or not.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Termbases can be read-only, i.e. not even an administrative user can get write access, export entries, etc. This is the case for termbases provided by publishing houses such as Langenscheidt. Using this property you can ascertain whether a particular termbase is read-only. If this is the case, you can, for example, disable edit commands of your client application.



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];
bool bReadOnly = oTb.IsReadOnly;

if(bReadOnly)
{
   	//disable edit button
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.IsReadOnly)

