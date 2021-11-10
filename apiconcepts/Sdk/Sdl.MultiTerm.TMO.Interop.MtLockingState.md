

# 
    Sdl.MultiTerm.TMO.Interop.MtLockingState Enumeration




## Name

Sdl.MultiTerm.TMO.Interop.MtLockingState —          Contains the possible values for locking operations.



## Description


.md)
Using the [LockEntry](Sdl.MultiTerm.TMO.Interop.Entry.LockEntry.md) you can lock or unlock entries, depending on which value you provide as parameter.



## Values

* *mtLock*

    Used for locking a particular entry, so that while the entry is being edited no other users can get write access to it.
* *mtUnlock*

    Releases the entry lock. Note that the entry lock is released automatically after applying the [Update](Sdl.MultiTerm.TMO.Interop.EntryContent.Update.md) method, i.e. normally you won't have to release the lock explicitly.




## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.MtLockingState)

