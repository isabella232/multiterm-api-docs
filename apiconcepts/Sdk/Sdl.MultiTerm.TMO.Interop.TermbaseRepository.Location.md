# Location property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.Location —          Sets/returns the location of a termbase server.

## Type

String
(read / write)

## Index Parameters
*none*

## Description

The location of a MultiTerm server corresponds to the name (or IP address) of the server machine. This parameter is required, so that the client application 'knows' to which server a connection should be established.

Examples:
```cs

.Location = "http://serv0234"
```

or
```cs
.Location = "http://www.multiterm.com"
```
or
```cs
.Location = "http://216.116.51.53"
```
For the local repository, this property contains the name of the local machine and is not used internally.

## Sample


```cs
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location = "http://ServerName";
oServRep.Connect("username", "password");
```


