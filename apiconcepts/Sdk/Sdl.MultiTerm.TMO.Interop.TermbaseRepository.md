

# 
    Sdl.MultiTerm.TMO.Interop.TermbaseRepository class




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository —          Provides access to the termbase repositories.



## Description

A MultiTerm client application has access to two termbase repositories: a local repository  (your hard disk) and a (remote) server repository. The local repository provides  access to all termbases stored locally in \*.sdltb format, whereas the server repository contains termbases hosted on a remote server in Oracle or SQL Server database format.

You can access the list of termbases in a server repository once you connected to it. The local repository, on the other hand, is initially empty and you have to add termbases to work with them. It will not remember a list of previoulsly used \*.sdltb files, that's the responsibility of the application using the API.



## Properties
.md)
* [DatabaseType](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.DatabaseType.md): Returns the database backend type for the current connection.
* [IsConnected](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.IsConnected.md): Indicates whether a connection has been established successfully.
* [IsRemote](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.IsRemote.md): Returns whether a connection is remote.
* [Location](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Location.md): Sets/returns the location of a termbase server.
* [Termbases](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Termbases.md): Provides access to the termbases contained in a local or server repository.




## Methods

* [ChangePassword](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.ChangePassword.md): Changes the password of the currently logged-in user.
* [Connect](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Connect.md): Connects to a MultiTerm Server.
* [Disconnect](Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Disconnect.md): Disconnects from a  MultiTerm Server.




## Sample


```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oLocalRep = oMt.LocalRepository;	
TermbaseRepository oServerRep = oMt.ServerRepository;
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository)

