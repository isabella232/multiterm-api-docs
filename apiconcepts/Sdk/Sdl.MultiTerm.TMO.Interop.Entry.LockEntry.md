# LockEntry method
## Name

Sdl.MultiTerm.TMO.Interop.Entry.LockEntry —          Locks an entry for editing.


## Returntype
void



## Parameters
* LockState ([Sdl.MultiTerm.TMO.Interop.MtLockingState](Sdl.MultiTerm.TMO.Interop.MtLockingState.md)

## Description

When a user is editing an entry from a client application, the entry is locked for all other users, i.e. it cannot be edited by another user. This is to prevent the same entry from being edited by more than one user at the same time.

When you want to implement editing functionality in your client make sure that entries to be edited are always locked before the actual editing operation takes place. Otherwise an error will be thrown.

Note that the LockEntry method can also be used to unlock an entry. Whether an entry is locked by this method or not depends on the parameter you provide, i.e. mtLock or mtUnlock.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);

//lock entry
oEntry.LockEntry(Sdl.MultiTerm.TMO.Interop.MtLockingState.mtLock);
```

