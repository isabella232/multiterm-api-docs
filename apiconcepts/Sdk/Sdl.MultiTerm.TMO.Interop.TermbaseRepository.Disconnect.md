

# 
    Disconnect method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Disconnect —          Disconnects from a  MultiTerm Server.



## Returntype

void



## Parameters
*none*


## Description



Applying this method to a termbase repository will disconnect the current user from the MultiTerm Server. This method requires no parameters. It should be called, e.g. when closing the client application. The corresponding login will then be deleted on the MultiTerm server.



## Sample


```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location = "http://localhost";
oServRep.Connect("guest", "guest");

oServRep.Disconnect();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Disconnect)

