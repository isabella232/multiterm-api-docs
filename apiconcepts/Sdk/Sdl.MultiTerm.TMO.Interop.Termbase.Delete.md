# Delete method

## Important: Method is no longer supported

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.Delete —          Deletes a particular termbase.

## Returntype

void


## Parameters
*none*


## Description

Applying this method to a termbase object will physically delete the termbase. In case of local termbases the corresponding \*.mdb file will be deleted. In case of server termbases, only the reference to the termbase in the MtMaster database will be removed. The actual physical termbase will remain in the SQL Server or Oracle backend and can only be removed by the database backend administrator. Note that only administrative MultiTerm users can apply this method to a server termbase.


## Sample


```cs
Termbase oTb = oTbs[0];
oTb.Delete();
```