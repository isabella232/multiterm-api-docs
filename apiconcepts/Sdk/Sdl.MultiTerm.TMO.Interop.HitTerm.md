

# 
    Sdl.MultiTerm.TMO.Interop.HitTerm class




## Name

Sdl.MultiTerm.TMO.Interop.HitTerm —          Provides programmatic access to a particular hit term.



## Description



This class allows you to retrieve a particular hit term. You will usually avail of this class to retrieve information such as the actual hit term content, the associated entry id, etc. This is useful, for example, to fill a list control with the hit terms found.



## Properties
.md)
* [Index](Sdl.MultiTerm.TMO.Interop.HitTerm.Index.md): Returns the name of the index in which a hit term has been found.
* [ParentEntryID](Sdl.MultiTerm.TMO.Interop.HitTerm.ParentEntryID.md): Returns the entry id associated with a particular hit term.
* [SearchScore](Sdl.MultiTerm.TMO.Interop.HitTerm.SearchScore.md): Returns the fuzziness score for a particular hit term.
* [Termbase](Sdl.MultiTerm.TMO.Interop.HitTerm.Termbase.md): Returns the name of the termbase in which a hit term was found.
* [Text](Sdl.MultiTerm.TMO.Interop.HitTerm.Text.md): Returns the actual hit term.




## Methods
*None*


## Sample


```cs
Termbase oTb = oTbs["Termbase name"];
TermbaseSearch oSearch = oTb.Search;
oSearch.Direction=Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
oSearch.MaximumHits=10;
oSearch.SourceIndex="English";
oSearch.SearchExpression ="starship";

HitTerms oHits = oSearch.Execute();
HitTerm oHit;
for(int i=0;i<oHits.Count;i++)
{
   	oHit = oHits[i];
   	Debug.WriteLine(oHit.Text);
   	Debug.WriteLine(oHit.Termbase);
   	Debug.WriteLine(oHit.Index);
   	Debug.WriteLine(oHit.ParentEntryID);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.HitTerm)

