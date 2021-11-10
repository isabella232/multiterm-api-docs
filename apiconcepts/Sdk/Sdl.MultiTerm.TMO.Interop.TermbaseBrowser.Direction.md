

# 
    Direction property




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Direction —          Sets/returns the direction for a browse operation.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.MtBrowseDirection](Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.md)

(read / write)



## Index Parameters
*none*


## Description



A browse operation can either be performed in the up or down direction. Usually, a browse operation is done from the first term of an index towards the last term, i.e. normally you will set this parameter to down.



## Sample


```cs
TermbaseBrowser tbBrowse = oTb.Browse;

tbBrowse.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
tbBrowse.MaximumTermCount=1;
tbBrowse.SourceIndex="English";
tbBrowse.StartTerm="";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Direction)

