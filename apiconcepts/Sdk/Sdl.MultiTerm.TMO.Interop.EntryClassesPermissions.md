# Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions class


## Name 
Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions —          Provides programmatic access to the entry classes the currently logged-in user has access to.


## Description


Entry classes can be used to categorize entries. By default, each termbase has the entry classes 'Unspecified', 'Public', and 'Internal'. Termbase administrators can add other entry classes such as 'Confidential', 'Secret', etc. and then restrict access to specific entries for user roles based on these entry classes.

Via the EntryClassesPermissions class you can, for example, ascertain to which entry classes the currently logged-in user has access.


## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.Count.md): Returns the number of entry classes a user has access to.
* [Item](Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.Item.md): Refers to a specific entry class.
* [XML](Sdl.MultiTerm.TMO.Interop.EntryClassesPermissions.XML.md): Returns all entry class permissions as an XML string.




## Methods
*None*


## Sample


```cs
//select termbase
Termbase oTb = oTbs["TRADOS"];

//retrieve the termbase access permissions of the currently logged-in user
TermbaseAccessPermissions oPermissions = oTb.AccessPermissions;
EntryClassesPermissions oClasses = oPermissions.EntryClasses;
Debug.WriteLine("Number of accessible entry classes: " + oClasses.Count.ToString());

oServerRep.Disconnect();
```

