

# 
    StartTerm property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.StartTerm —          Sets/returns the start term for the browse operation.



## Type

String

(read / write)



## Index Parameters
*none*


## Description



A browse operation is executed in a specified termbase index (i.e. language) starting from a particular term. For example, if the start term is "apple", the following term that is retrieved through the browse operation might be "apricot" or "banana". If "network" has been specified as the start term, the browse operation might retrieve the term "ODBC", etc.

Via the StartTerm property you determine the position of the index (i.e. the term) from which the browse operation should take place. Instead of an entire term you may also specify only part of a term or just a letter, e.g. "a".

If this parameter is not specified an empty value ("") will be used by default. This means that the browse operation will start from the very beginning of the index.

If the specified term does not exist in the termbase, the alphabetically nearest term is used as a starting point instead.



## Sample


```cs
TermbaseBrowser tbBrowse = oTb.Browse;

tbBrowse.StartTerm="";
tbBrowse.Direction = Sdl.MultiTerm.TMO.Interop.MtBrowseDirection.mtBrowseDown;
tbBrowse.SourceIndex="English";
tbBrowse.MaximumTermCount=1;
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseBrowser.StartTerm)

