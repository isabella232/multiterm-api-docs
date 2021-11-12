# DefaultEntryClass property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.DefaultEntryClass —          Returns the default entry class for a particular termbase.

## Type

String
(read)

## Index Parameters
*none*

## Description

Entry classes are a way of classifying entries. Using entry classes it is possible to restrict user access to certain entries. Entry classes are only available for server-based termbases.

Each server-based termbase has a default entry class, which is automatically applied to every new entry unless another entry class has been specified. The default entry class is usually "Unspecified", however, the termbase administrator can also select a different entry class.

This property is used to determine the default entry class of a particular termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

Debug.Write("Default entry class name: " + oTb.DefaultEntryClass);
```

