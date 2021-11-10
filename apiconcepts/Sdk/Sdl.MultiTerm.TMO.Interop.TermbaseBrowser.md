

# 
    Sdl.MultiTerm.TMO.Interop.TermbaseBrowser class




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser —          Provides access to the browse functionality for a termbase.



## Description



Browsing a termbase involves navigating to the next or previous entry (or entries) starting from a particular position in the browse index (i.e. the currently selected source index).

This class allows you to implement browse functionality for your MultiTerm client application. A browse operation requires various parameters, such as the browse direction (up/down), the browse index (language), the maximum number of terms to retrieve with a browse operation, etc.



## Properties
.md)
* [Direction](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Direction.md): Sets/returns the direction for a browse operation.
* [EntryID](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.EntryID.md): Sets/returns the starting entry id of the browse operation.
* [MaximumTermCount](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.MaximumTermCount.md): Sets/returns the maximum hits allowed for a browse operation.
* [SourceIndex](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.SourceIndex.md): Sets/returns the browse index.
* [StartTerm](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.StartTerm.md): Sets/returns the start term for the browse operation.




## Methods

* [Execute](Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Execute.md): Executes the browse operation.




## Sample


```cs
TermbaseBrowser tbBrowse = oTb.Browse;

tbBrowse.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
tbBrowse.SourceIndex="English";
tbBrowse.StartTerm="";
tbBrowse.MaximumTermCount=1;

HitTerms oHits = tbBrowse.Execute();
Debug.Write("Browse hit: " + oHits[0].Text);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser)

