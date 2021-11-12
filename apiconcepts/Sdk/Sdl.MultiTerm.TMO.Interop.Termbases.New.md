# New method

## Name

Sdl.MultiTerm.TMO.Interop.Termbases.New —          Creates a new termbase programmatically.

## Returntype
[Sdl.MultiTerm.TMO.Interop.Termbase](Sdl.MultiTerm.TMO.Interop.Termbase.md)


## Parameters

* TermbaseName (String, *optional*)
* Description (String, *optional*)
* TermbaseDefinitionFile (String, *optional*)
* TermbaseDestinationFile (String, *optional*)

## Description

Applying this method to a (local or server) repository creates a new termbase. This method requires the name of the new termbase, an optional description as well as the path and name of the termbase definition file (\*.xdt) as parameters. In addition, local termbases require the path to the created .sdltb file.

If you do not specify an xdt file, or an empty string, an interactive wizard is started to collect the details.

Note that for creating server termbases an administrative login is required.

## Sample


```cs
TermbaseRepository oLocalRep = oMt.LocalRepository;
oLocalRep.Connect("", "");

Termbases oTbs = oLocalRep.Termbases;

oTbs.New("New Termbase File Name", "Optional Description", "c:\\temp\\test.xdt","c:\\temp\\test.sdltb");
MessageBox.Show("Termbase created successfully.");
```
