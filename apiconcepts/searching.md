# Searching a Termbase

The **TermbaseSearch** class allows you to programmatically perform a search in a particular termbase.  When searching a termbase you need to provide a number of parameters such as the search term, the search index,  the maximum number of terms that the search should yield, etc.  Below you find a sample code that shows you how to set the required parameters for a fuzzy search:


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
//set search parameters
TermbaseSearch search = oTb.Search;
search.Direction = Sdl.MultiTerm.TMO.Interop.MtSearchDirection.mtSearchDown;
search.MaximumHits = 10;
search.FuzzySearch = true;
search.SearchExpression = "search term";
search.SourceIndex = "English";
```

To carry out the search operation you need to apply the **Execute **method to the search, which returns a **HitTerms **object. This object can then be used to retrieve the hits found (if any). That way you can fill, e.g. a list control with the hits found during the search. The sample code below shows you how to carry out the search and how to output the search results:


```cs
HitTerms oHits = search.Execute();
Debug.WriteLine("Total hit count: " + oHits.ToString());
foreach(HitTerm oHit in oHits)
{
   Debug.WriteLine(oHit.Text);
} 
```


