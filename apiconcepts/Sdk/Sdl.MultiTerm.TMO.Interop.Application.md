# Sdl.MultiTerm.TMO.Interop.Application class

## Name

Sdl.MultiTerm.TMO.Interop.Application —  Provides programmatic access to the MultiTerm client functionality.



## Description

Creating an instance of the MultiTerm client application, which is the root of the MultiTerm object hierarchy, will allow a user to access the MultiTerm client functionality that is available with his/her particular login, e.g. searching in termbases, browsing termbases, editing termbase content, etc.

Below you find the minimum amount of C# code needed to create an instance of the MultiTerm Client object.

## Properties

* [LocalRepository](Sdl.MultiTerm.TMO.Interop.Application.LocalRepository.md): Provides access to all locally stored termbases.
* [MultiSearch](Sdl.MultiTerm.TMO.Interop.Application.MultiSearch.md): Provides programmatic access to multiple termbase search.
* [ServerRepository](Sdl.MultiTerm.TMO.Interop.Application.ServerRepository.md): Provides access to the termbases stored on a MultiTerm Server.


## Methods
*None*

## Sample

```cs
using System;
using MultiTermIX;

namespace MtSDKTest
{
   	class MtTest
   	{
      		[STAThread]
      		static void Main(string[] args)
      		{
         			Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
      		}
   	}
}
```


