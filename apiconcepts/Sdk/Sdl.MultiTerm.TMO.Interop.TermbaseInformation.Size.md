#  Size property

## Name

Sdl.MultiTerm.TMO.Interop.TermbaseInformation.Size —          Returns the size of the termbase in MB.

## Type

String
(read)


## Index Parameters
*none*

## Description

This property is used to retrieve the termbase size, i.e. the amount of physical hard disk space occupied by the termbase.

Note: This property does not apply to termbases hosted on Oracle backends.


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseInformation tbInfo = oTb.Information;
Debug.Write("Termbase size in MB: " + tbInfo.Size.ToString());
```

