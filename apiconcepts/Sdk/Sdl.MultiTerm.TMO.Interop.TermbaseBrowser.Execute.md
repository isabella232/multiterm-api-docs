

# 
    Execute method




## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Execute —          Executes the browse operation.



## Returntype
.md)
[Sdl.MultiTerm.TMO.Interop.HitTerms](Sdl.MultiTerm.TMO.Interop.HitTerms.md)



## Parameters
*none*


## Description



This method is applied to the Browse object to actually carry out the browse operation. The results of the browse operation (if any) are stored in a HitTerms object, from which the hit term(s) can subsequently be retrieved.

You need to set the SourceIndex and MaximumTermCount properties before calling Execute().



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];
TermbaseBrowser oBrowser = oTb.Browse;
oBrowser.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
oBrowser.MaximumTermCount = 1;
oBrowser.StartTerm="";
oBrowser.SourceIndex="English";

HitTerms oHits = oBrowser.Execute();
Debug.Write(oHits[0].Text);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.Execute)

