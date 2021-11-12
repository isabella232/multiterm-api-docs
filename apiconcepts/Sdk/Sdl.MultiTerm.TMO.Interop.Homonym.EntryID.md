# EntryID property

## Name

Sdl.MultiTerm.TMO.Interop.Homonym.EntryID —          Returns the entry id of a particular homonym.

## Type

Long
(read)

## Index Parameters
*none*

## Description

Via the entry id you can refer to a specific termbase entry and retrieve its content. This can be useful for seeing whether the selected homonym term belongs to a different concept or is an actual duplicate, and therefore redundant.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");

//select first homonym term
Homonym oHomonym = oHomonyms[0];
Debug.Write("Homonym entry id: " + oHomonym.EntryID.ToString());
```

