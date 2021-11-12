#  DatabaseType property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.DatabaseType —          Returns the database backend type for the current connection.

## Type

[Sdl.MultiTerm.TMO.Interop.MtDatabaseType](Sdl.MultiTerm.TMO.Interop.MtDatabaseType.md)
(read / write)

## Index Parameters
*none*

## Description

This property returns mtJET if a local termbase repository is used, mtSQL for Microsoft SQL Server backends and mtOracle for Oracle backends.

## Sample

```cs
MessageBox.Show(oServRep.DatabaseType.ToString());
```

