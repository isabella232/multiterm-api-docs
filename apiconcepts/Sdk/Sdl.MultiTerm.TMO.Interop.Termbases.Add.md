

# 
    Add method



## Name

Sdl.MultiTerm.TMO.Interop.Termbases.Add —          Allows you to access local termbases programmatically.



## Returntype

void



## Parameters

* Path (String)
* Name (String) - deprecated (for legacy reasons only)
* Description (String) - deprecated (for legacy reasons only)




## Description



This method can only be applied to a local termbase repository. It is the programmatic equivalent of the "Open" command in MultiTerm.  It is used to  provide access to local termbases stored in JET format (\*.sdltb) via the local termbase repository.

This method requires the full path of the \*.sdltb file. It is then available  within the Termbases collection, and can be access via its full path as its  name.



## Sample


```cs
TermbaseRepository oLocalRep = oMt.LocalRepository;	
oLocalRep.Connect("", "");		

Termbases oTbs = oLocalRep.Termbases;

oTbs.Add("C:\\temp\\mytermbase.sdltb", "", "");

oTB = oTbs.Item("C:\\temp\\mytermbase.sdltb");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbases.Add)

