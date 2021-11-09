

# 
    LocalRepository property



## Name

MultiTermIX.Application.LocalRepository —          Provides access to all locally stored termbases.



## Type

[MultiTermIX.TermbaseRepository](MultiTermIX.TermbaseRepository.html)

(read)



## Index Parameters
*none*


## Description



Termbases can be stored locally on your hard disk. Local termbases are stored in \*.sdltb  file format. This class allows you to provide access to local termbases.

Note that before you can retrieve any local termbases, you need to connect to the local termbase repository using the [Connect](MultiTermIX.TermbaseRepository.Connect.html) method, even if local termbase access does not require any authentication. However, you can provide an empty user name and password.



## Sample


```cs
MultiTermIX.Application oMt = new MultiTermIX.ApplicationClass();
TermbaseRepository oLocRep = oMt.LocalRepository;
oLocRep.Connect("", "");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20MultiTermIX.Application.LocalRepository)

