#  GetCrossLinkedEntry method


## Name

Sdl.MultiTerm.TMO.Interop.Entries.GetCrossLinkedEntry —          Allows you to retrieve the content of a cross-linked entry.

## Returntype

String

## Parameters

* Index (Variant)
* Term (String)
* CurrentEntryId (Long)

## Description

You can use this method to retrieve the content of an entry that is linked to another entry, thereby implementing a cross-reference functionality. In the MultiTerm XML cross-links look as follows:

DisplayTerm

A cross-link is made up of the index name the cross-linked term belongs to, the actual cross-linked term and the display text. The display text is often identical to the cross-linked term.

The GetCrossLinkedEntry method requires the index, the cross-linked term and the current entry id as parameters. The method returns the content of the entry that contains the cross-linked entry as an XML stream.


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//current entry has entry #1
Entry thisEntry = oEntries.Item(1);
//output content of cross-linked entry
Debug.Write(oEntries.GetCrossLinkedEntry("English", "starship", 17));
```


