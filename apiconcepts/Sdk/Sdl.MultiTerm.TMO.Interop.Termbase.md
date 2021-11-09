

# 
    Sdl.MultiTerm.TMO.Interop.Termbase class



## Name

Sdl.MultiTerm.TMO.Interop.Termbase —          Provides programmatic access to a particular termbase.



## Description



A termbase is a database that is physically stored in a JET, SQL Server or Oracle backend. A termbase contains a number of entries (i.e. concepts), a set of so-called termbase or catalog objects (e.g. filter and layout definitions, etc.) and possibly also multimedia blobs.

The Termbase class allows you to retrieve various information on a specified termbase, e.g. the termbase name, location, the entry count, the number of indexes in the termbase definition, etc.

Apart from that you can also configure a number of settings for a selected termbase, e.g. the source and target index, the active filter, etc.

To select a termbase from a termbase repository you can either use the termbase path (for local termbases), the termbase name (for server termbases) or the index number, e.g.:

oTb = oTbs["C:\Testdata\Sample Termbase.sdltb"] or

oTb = oTbs["Sample Termbase"] or

oTb = oTbs[0]



## Properties

* [\_Cookie](Sdl.MultiTerm.TMO.Interop.Termbase._Cookie.html): [For internal use only.]
* [\_DefaultEntryClassID](Sdl.MultiTerm.TMO.Interop.Termbase._DefaultEntryClassID.html): Returns the default entry class id.
* [\_IsLocal](Sdl.MultiTerm.TMO.Interop.Termbase._IsLocal.html): Flags whether a termbase is local or not.
* [AccessPermissions](Sdl.MultiTerm.TMO.Interop.Termbase.AccessPermissions.html): Provides programmatic access to the permissions the currently logged-in user has to a termbase.
* [ActiveFilter](Sdl.MultiTerm.TMO.Interop.Termbase.ActiveFilter.html): Returns the active filter for a termbase.
* [Browse](Sdl.MultiTerm.TMO.Interop.Termbase.Browse.html): Provides access to the browse functionality for a termbase.
* [ChangeDate](Sdl.MultiTerm.TMO.Interop.Termbase.ChangeDate.html): Returns the last termbase change date.
* [CopyrightText](Sdl.MultiTerm.TMO.Interop.Termbase.CopyrightText.html): Returns the copyright text for a particular termbase.
* [DefaultEntryClass](Sdl.MultiTerm.TMO.Interop.Termbase.DefaultEntryClass.html): Returns the default entry class for a particular termbase.
* [Definition](Sdl.MultiTerm.TMO.Interop.Termbase.Definition.html): Provides programmatic access to a termbase definition.
* [DownloadedCopyrightIcoPath](Sdl.MultiTerm.TMO.Interop.Termbase.DownloadedCopyrightIcoPath.html): Returns the path and name of the termbase icon file.
* [DownloadedCopyrightInfoPath](Sdl.MultiTerm.TMO.Interop.Termbase.DownloadedCopyrightInfoPath.html): Returns the path and name of the termbase reference document.
* [DownloadedCopyrightSplashPath](Sdl.MultiTerm.TMO.Interop.Termbase.DownloadedCopyrightSplashPath.html): Returns the path and name of the termbase splash screen image.
* [Entries](Sdl.MultiTerm.TMO.Interop.Termbase.Entries.html): Provides programmatic access to the entries of a termbase.
* [ExpiryDate](Sdl.MultiTerm.TMO.Interop.Termbase.ExpiryDate.html): Returns the expiry date of the termbase.
* [ExportDefinitions](Sdl.MultiTerm.TMO.Interop.Termbase.ExportDefinitions.html): Provides programmatic access to the export definitions of a termbase.
* [FilterDefinitions](Sdl.MultiTerm.TMO.Interop.Termbase.FilterDefinitions.html): Provides programmatic access to the filter definitions of a termbase.
* [ImportDefinitions](Sdl.MultiTerm.TMO.Interop.Termbase.ImportDefinitions.html): Provides programmatic access to the filter definitions of a termbase.
* [IncompleteEntries](Sdl.MultiTerm.TMO.Interop.Termbase.IncompleteEntries.html): Provides programmatic access to the incomplete entries of a termbase.
* [Information](Sdl.MultiTerm.TMO.Interop.Termbase.Information.html): Provides programmatic access to the termbase information.
* [InputModelDefinitions](Sdl.MultiTerm.TMO.Interop.Termbase.InputModelDefinitions.html): Provides programmatic access to the input model definitions of a termbase.
* [IsReadOnly](Sdl.MultiTerm.TMO.Interop.Termbase.IsReadOnly.html): Returns True or False depending on whether a termbase is read-only or not.
* [LayoutDefinitions](Sdl.MultiTerm.TMO.Interop.Termbase.LayoutDefinitions.html): Provides programmatic access to the layout definitions of a termbase.
* [LockedEntries](Sdl.MultiTerm.TMO.Interop.Termbase.LockedEntries.html): Provides programmatic access to the locked entries of a termbase.
* [Name](Sdl.MultiTerm.TMO.Interop.Termbase.Name.html): Returns the name of a termbase.
* [Search](Sdl.MultiTerm.TMO.Interop.Termbase.Search.html): Provides programmatic access to the search functionality for a particular termbase.




## Methods

* [\_Reorganise](Sdl.MultiTerm.TMO.Interop.Termbase._Reorganise.html): [For internal use only.]
* [Close](Sdl.MultiTerm.TMO.Interop.Termbase.Close.html): Closes a specified termbase.
* [Delete](Sdl.MultiTerm.TMO.Interop.Termbase.Delete.html): Deletes a particular termbase.
* [ExtractToFile](Sdl.MultiTerm.TMO.Interop.Termbase.ExtractToFile.html): Saves the a termbase to an \*.mdb file.
* [GetHomonyms](Sdl.MultiTerm.TMO.Interop.Termbase.GetHomonyms.html): Retrieves all homonym entries of a particular termbase.
* [Reorganise](Sdl.MultiTerm.TMO.Interop.Termbase.Reorganise.html): Reorganises a specified termbase.




## Sample


```cs
Termbases oTbs = oLocalRep.Termbases;
Termbase oTb = oTbs["Termbase Path"];

Debug.Write("Total number of termbase entries: " + oTb.Information.TotalNumberOfEntries.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase)

