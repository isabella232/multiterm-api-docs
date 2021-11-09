

# 
    Term property



## Name

Sdl.MultiTerm.TMO.Interop.Homonym.Term —          Returns the homonym term.



## Type

String

(read)



## Index Parameters
*none*


## Description



This property allows you to output the actual homonym term(s) that was/were found in a particular termbase index. This is useful, e.g. for generating a list of homonym terms.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");

//select first homonym term
Homonym oHomonym = oHomonyms[0];
Debug.Write("Homonym term: " + oHomonym.Term);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Homonym.Term)

