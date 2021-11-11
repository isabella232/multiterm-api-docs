# LocalRepository property

## Name

Sdl.MultiTerm.TMO.Interop.Application.LocalRepository —          Provides access to all locally stored termbases.

## Type

[Sdl.MultiTerm.TMO.Interop.TermbaseRepository](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.md)

(read)

## Index Parameters
*none*


## Description

Termbases can be stored locally on your hard disk. Local termbases are stored in \*.sdltb  file format. This class allows you to provide access to local termbases.

Note that before you can retrieve any local termbases, you need to connect to the local termbase repository using the [Connect](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Connect.md) method, even if local termbase access does not require any authentication. However, you can provide an empty user name and password.



## Sample

```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oLocRep = oMt.LocalRepository;
oLocRep.Connect("", "");
```


