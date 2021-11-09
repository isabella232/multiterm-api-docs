
# Retrieving Entry Content

MultiTerm entries are physically stored as XML blobs in the database backend. Retrieving an entry basically involves retrieving the XML content from the database. Once you have retrieved the content of an entry, you can, for example, parse it using the DOM API, apply an XSL stylesheet to it for transformation, etc.

In the first step you need to create a termbase entries collection object using the **Entries** class, e.g.:


```cs
Entries oEntries = oTermbase.Entries;
```

To pick a particular entry, you need to provide the corresponding entry id. The entry id is used to uniquely identify an entry, e.g.:


```cs
Entry oEntry = oEntries.Item(5);
```

The above sample code selects the entry with the id 5. Take care to provide only entry ids that actually exist in the termbase. Otherwise, an exception will be thrown. The entry content can be retrieved in the following way:


```cs
Debug.Write(oEntry.Content.Content);
```

The above line will output the complete entry XML content. Let's take this one step further: suppose you would like to develop a MultiTerm client application that allows users to display the entire entry by clicking the corresponding hit term in the hit list. This can be done easily, as the **HitTerm **object allows you to retrieve the id of the entry a hit term comes from. Example:


```cs
HitTerms oHits = oSearch.Execute();
  Debug.WriteLine("Hit count: " + oHits.Count.ToString());
  for(int i=0;i<oHits.Count;i++)
  {
   Debug.WriteLine(oHits[i].Text);
   //retrieve entry id for current hit term
   int thisEntryId = Convert.ToInt32(oHits[i].ParentEntryID);
   oEntry = oEntries[thisEntryId];
   //output content of current entry
   Debug.WriteLine(oEntry.Content.Content);
}
```

The above sample code executes a search and stores the search results in a **HitTerms** object. The code then loops through all hits, retrieves the entry id of each hit, and then outputs the entire entry content for each hit term.




