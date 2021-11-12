#  NumberOfEntriesInIndex property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.NumberOfEntriesInIndex —          Returns the number of terms contained in a specified index.

## Type

Long
(read)

## Index Parameters

* Index (String)

## Description

This property allows you to ascertain the number of terms of a particular index. Note that the term count of an index can be bigger than the total termbase entry count, as indexes can contain a number of synonyms.

The index name has to be provided as string parameter.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Number of terms in the English index: " + tbInfo.get_NumberOfEntriesInIndex("English"));
```

