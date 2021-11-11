# ApplyFilter method

## Name

Sdl.MultiTerm.TMO.Interop.Entry.ApplyFilter —          Applies a filter definition to a specified entry and returns True or False, depending on whether the entry matches the filter.

## Returntype
Boolean


## Parameters
* FilterObject ([Sdl.MultiTerm.TMO.Interop.FilterDefinition](Sdl.MultiTerm.TMO.Interop.FilterDefinition.md)
* SourceIndex (String, *optional, default is ""*)
* TargetIndex (String, *optional, default is ""*)




## Description

Filters are used to search for a subset of entries in the termbase, e.g. all entries that were created after a specified date, all entries that contain or do not contain a certain field, etc.

By applying this method to particular entry you can determine whether the entry matches the filter or not.

This method is useful, if you want e.g. to iterate through all entries in a termbase and then apply this method to each entry to check whether it matches the filter. You may then process all matching entries in a particular way, e.g. insert them into a Word document, etc.

This method requires a filter object as parameter. Filters can be selected either via the corresponding index number or via the unique termbase object name, which is case-sensitive, e.g. Filter["Missing Target"] or Filter[0].

Additionally, this method requires the source and target index, as filter definitions may use the source and/or target index as criteria, e.g. a filter that looks for all entries where the target term is missing. This method returns true if the entry is matching the filter, false if not.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);

//select export definition
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

//apply export definition
Debug.Write("Entry matches filter: "  + oEntry.ApplyFilter(oFilter, "English", "German"));
```