

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.Termbases.Count —          Returns the number of available termbases.



## Type

Long

(read)



## Index Parameters
*none*


## Description



This property is used to determine the number of termbases available in either the local or the server termbase repository. Note that for server termbases it will only return the number of termbases you have access to with your current login.



## Sample


```cs
Termbases oTbs = oServRep.Termbases;
MessageBox.Show(oTbs.Count.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbases.Count)

