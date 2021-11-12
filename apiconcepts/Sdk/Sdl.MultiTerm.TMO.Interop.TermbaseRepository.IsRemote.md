# IsRemote property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.IsRemote —          Returns whether a connection is remote.

## Type
Boolean
(read)

## Index Parameters
*none*

## Description


This property is used to check whether a connection is remote or not. For connections to a local termbase repository this property will return the value False.

You can use this property, for example, to check whether a user name and password is required for a connection, which is not the case for local connections.

## Sample


```cs
MessageBox.Show("Is remote: " + oTbRep.IsRemote);
```
