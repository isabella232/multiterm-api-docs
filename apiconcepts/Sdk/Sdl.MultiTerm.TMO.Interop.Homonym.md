

# 
    Sdl.MultiTerm.TMO.Interop.Homonym class




## Name

Sdl.MultiTerm.TMO.Interop.Homonym —          Provides programmatic access to a particular homonym in the termbase.



## Description



Via this class you can retrieve information on a selected homonym term. This will usually be the actual term itself and the entry number.

The sample code below retrieves all homonyms from the "English" index, then selects the first homonym term and then the second.

Note that via referring to the unique entry id, you can retrieve the content of an entire entry. This can be useful for implementing a function that lists all homonyms of a particular index. By clicking a homonym entry id, the user can display the entire entry and thus ascertain whether the homonym is a (redundant) duplicate or is a real homonym, i.e. the same term having different meanings (e.g. 'book' a flight and read a 'book').



## Properties
.md)
* [EntryID](Sdl.MultiTerm.TMO.Interop.Homonym.EntryID.md): Returns the entry id of a particular homonym.
* [Index](Sdl.MultiTerm.TMO.Interop.Homonym.Index.md): Returns the index the homonym term was found in.
* [Term](Sdl.MultiTerm.TMO.Interop.Homonym.Term.md): Returns the homonym term.




## Methods
*None*


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

Homonyms oHomonyms = oTb.GetHomonyms("English", "","");

//select first homonym term
Homonym oHomonym = oHomonyms[0];
Debug.Write("Homonym term: " + oHomonym.Term);
Debug.Write("Homonym entry id: " + oHomonym.EntryID.ToString());

//select second homonym term
oHomonym = oHomonyms[1];
Debug.Write("Homonym term: " + oHomonym.Term);
Debug.Write("Homonym entry id: " + oHomonym.EntryID.ToString());
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Homonym)

