#  StartWizard method

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.StartWizard —          Calls the Termbase Definition Wizard.

## Returntype

void

## Parameters
*none*

## Description

Applying this method to a TermbaseDefinition object will call up the Termbase Definition Wizard, which allows you to modify the selected termbase definition in the wizard GUI. Note that for server termbases, administrator access is required to edit a termbase definition.

## Sample


```cs
Termbase oTb = oTbs[0];

TermbaseDefinition tbDef = oTb.Definition;
tbDef.StartWizard();
```
