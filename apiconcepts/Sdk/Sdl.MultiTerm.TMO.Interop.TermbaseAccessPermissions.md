#  Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions class

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions —          Provides programmatic access to the termbase access permissions of the currently logged-in user.

## Description


Via this class you can, for example, determine whether the currently logged-in user is allowed to change the value of entry classes, ascertain which indexes the user can access etc. One possible application is the generation of a list that contains only the indexes that a user has access to.


## Properties
* [CanChangeEntryClass](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.CanChangeEntryClass.md): Returns whether the currently-logged in user can change entry class values.
* [CanExport](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.CanExport.md): Returns true or false depending on whether the current user has export privileges or not.
* [CanImport](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.CanImport.md): Returns true or false depending on whether the current user has import privileges or not.
* [EntryClasses](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryClasses.md): Provides programmatic access to the entry classes the currently logged-in user has access to.
* [EntryLevelRead](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryLevelRead.md): Returns true if the currently logged-in user has read access to entry-level fields.
* [EntryLevelWrite](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.EntryLevelWrite.md): Returns true if the currently logged-in user has write access to entry-level fields.
* [IndexesPermissions](Sdl.MultiTerm.TMO.Interop.TermbaseAccessPermissions.IndexesPermissions.md): Provides access to the indexes that the currently logged-in user can access.


## Methods
*None*

## Sample

```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
Debug.WriteLine(oPermissions.CanChangeEntryClass);
Debug.WriteLine("Number of indexes the user can access: " + oPermissions.IndexesPermissions.Count.ToString());
```
