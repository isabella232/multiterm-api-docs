

# 
    Protocol property




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Protocol —          Provides access to the protocol types that can be used to connect to a MultiTerm server.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.MtCommunicationType](Sdl.MultiTerm.TMO.Interop.MtCommunicationType.md)

(read / write)



## Index Parameters
*none*


## Description



Connections to a remote termbase server can be made through the DCOM protocol (LAN environments) or using the SOAP protocol (WAN scenarios).

This enumerator contains the possible protocol type values used when providing the information required to connect to a termbase server.



## Sample


```cs
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location ="ServerName";
oServRep.Protocol = Sdl.MultiTerm.TMO.Interop.MtCommunicationType.mtDCOM;
oServRep.Connect("username", "password");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Protocol)

