

# 
    Connect method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Connect —          Connects to a MultiTerm Server.



## Returntype

[Sdl.MultiTerm.TMO.Interop.MtUserType](Sdl.MultiTerm.TMO.Interop.MtUserType.html)



## Parameters

* UserId (String)
* Password (String)




## Description



Applying this method to a termbase repository will establish a connection to the corresponding repository, allowing you to gain access to the termbases that you are allowed to see with your current login.

This method requires the user name and password as string parameters.

To access file based termbases, through the local repository, set user and password to "" (empty string).



## Sample


```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location = "http://localhost";
oServRep.Connect("username", "password");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Connect)

