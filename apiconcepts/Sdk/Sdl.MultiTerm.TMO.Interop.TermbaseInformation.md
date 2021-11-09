

# 
    Sdl.MultiTerm.TMO.Interop.TermbaseInformation class



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation —          Provides programmatic access to a set of termbase information.



## Description



This class allows you to retrieve various items of information on a particular termbase, e.g. the termbase size, full name, total number of entries, etc.

You can use this class, for example, to display all relevant termbase information in a termbase information frame whenever a user selects a termbase name from a list.



## Properties

* [CreationDate](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.CreationDate.html): Returns the termbase creation date.
* [Description](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Description.html): Returns the termbase description.
* [Name](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Name.html): Returns the (nice) name of a termbase.
* [NumberOfEntriesInIndex](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.NumberOfEntriesInIndex.html): Returns the number of terms contained in a specified index.
* [Size](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Size.html): Returns the size of the termbase in MB.
* [TotalNumberOfEntries](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.TotalNumberOfEntries.html): Returns the total entry count for the specified termbase.




## Methods

* [Refresh](Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Refresh.html): Updates the termbase information.




## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Termbase description: " + tbInfo.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseInformation)

