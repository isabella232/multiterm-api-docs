# Item property

## Name

Sdl.MultiTerm.TMO.Interop.LockedEntries.Item —          Provides access to a particular locked entry.

## Type

String
(read)

## Index Parameters

* Index (Long)

## Description

Via this property you can access a specific locked entry to retrieve further information such as the time the entry was locked and the name of the user by whom it was locked.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LockedEntries oLocks = oTb.LockedEntries;
//select first locked entry
LockedEntry oLock = oLocks[0];
```
