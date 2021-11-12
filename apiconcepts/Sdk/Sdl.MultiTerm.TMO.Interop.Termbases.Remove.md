# Remove method

## This method is no longer supported.

## Name

Sdl.MultiTerm.TMO.Interop.Termbases.Remove —          Removes a termbase from a local termbase collection.

## Returntype
void

## Parameters
* Termbase ([Sdl.MultiTerm.TMO.Interop.Termbase](Sdl.MultiTerm.TMO.Interop.Termbase.md))
* DestinationPath (String)

## Description
Applying this method removes a specified termbase from a local termbase collection without however deleting the physical termbase (\*.mdb) file. It is the programmatic equivalent of the "Detach" command in MultiTerm Workstation. The method requires the termbase object to remove and the path to which a copy (i.e. an\*. mdb file) of the removed termbase should be saved

## Sample


```cs
TermbaseRepository oLocalRep = oMt.LocalRepository;	
oLocalRep.Connect("", "");		

Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs["New Termbase Name"];
oTbs.Remove(oTb, "c:\\temp\\");
MessageBox.Show("Termbase removed successfully.");
```
