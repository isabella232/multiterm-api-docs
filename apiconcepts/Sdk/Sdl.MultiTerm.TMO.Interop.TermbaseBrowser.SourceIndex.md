

# 
    SourceIndex property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.SourceIndex —          Sets/returns the browse index.



## Type

String

(read / write)



## Index Parameters
*none*


## Description



A browse operation is always performed in a particular index (language). Use this property to set the browse index to the required language, e.g. 'English'.



## Sample


```cs
TermbaseBrowser tbBrowse = oTb.Browse;

tbBrowse.SourceIndex="English";
tbBrowse.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
tbBrowse.StartTerm="";
tbBrowse.MaximumTermCount=1;
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.SourceIndex)

