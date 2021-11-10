# Sdl.MultiTerm.TMO.Interop.DescriptiveFields class

## Name

Sdl.MultiTerm.TMO.Interop.DescriptiveFields —  Provides programmatic access to the descriptive fields of a termbase definition.

## Description

You can use this class, for example, to generate a list of all entry-level descriptive fields of a particular termbase definition.

## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Count.md): Returns the number of entry-level descriptive fields.
* [Item](Sdl.MultiTerm.TMO.Interop.DescriptiveFields.Item.md): Provides access to a particular entry-level descriptive fields.

## Methods
*None*

## Sample

```cs
TermbaseDefinition tbDef = oTb.Definition;
DescriptiveFields oDFields = tbDef.Fields;
Debug.Write("Descriptive field count: " + oDFields.Count.ToString());
```
