

# 
    Termbases property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Termbases —          Provides access to the termbases contained in a local or server repository.



## Type

[Sdl.MultiTerm.TMO.Interop.Termbases](Sdl.MultiTerm.TMO.Interop.Termbases.html)

(read)



## Index Parameters
*none*


## Description



You can use this class, e.g. to generate a list of available termbases, so that the client user can choose one or several termbases to access.



## Sample


```cs
Termbases oTbs = oServRep.Termbases;

for(int i=0;i<oTbs.Count;i++)
{
   	Debug.WriteLine("Termbase name: " + oTbs[i].Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Termbases)

