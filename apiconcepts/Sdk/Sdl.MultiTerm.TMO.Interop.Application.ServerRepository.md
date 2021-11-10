
# ServerRepository property

## Name

Sdl.MultiTerm.TMO.Interop.Application.ServerRepository —          Provides access to the termbases stored on a MultiTerm Server.

## Type

[Sdl.MultiTerm.TMO.Interop.TermbaseRepository](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.md)

(read)

## Index Parameters
*none*

## Description

Via this class you can access those termbases stored on a MultiTerm Server machine that your login allows you to access.

In order to access a MultiTerm Server you need to provide the server machine name and your user name and password.

## Sample

```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location = "http://localhost";
oServRep.Connect("guest", "guest");
MessageBox.Show ("Server termbase count: " + oServRep.Termbases.Count.ToString());

oServRep.Disconnect();
```
