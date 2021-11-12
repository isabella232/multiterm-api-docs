# ExtractToFile method

## This method is no longer supported

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.ExtractToFile —          Saves the a termbase to an \*.sdltb     file.

## Returntype

void


## Parameters

* bstr_localFile (String)



## Description


Applying this method to a local termbase saves it to a particular file on the user's hard disk. The actual termbase will still remain in the local termbase repository. This method requires the full name and path of the \*.mdb file to which the local termbase should be copied.

This method is useful when you want to have a physical termbase copy to forward to another user.



## Sample


```cs
Sdl.MultiTerm.TMO.Interop.ApplicationClass mt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
mt.LocalRepository.Connect("","");
Termbase myTermbase = mt.LocalRepository.Termbases["Termbase Name"];

myTermbase.ExtractToFile("c:\\temp\\extracted.mdb");
```
