

# 
    MaximumTermCount property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.MaximumTermCount —          Sets/returns the maximum hits allowed for a browse operation.



## Type

Long

(read / write)



## Index Parameters
*none*


## Description



This property is used to determine the maximum number of hits for a browse operation. To browse to the next or previous term you would set this parameter to 1. If you want to retrieve a number of terms from the current position, you would set this parameter to the corresponding number. For example, to retrieve the next 5 terms you would set this property to 5.



## Sample


```cs
TermbaseBrowser tbBrowse = oTb.Browse;

tbBrowse.MaximumTermCount=1;
tbBrowse.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
tbBrowse.SourceIndex="English";
tbBrowse.StartTerm="";
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.MaximumTermCount)

