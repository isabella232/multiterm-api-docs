

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.EntryIDs.Item —          Refers to a particular entry id.



## Type

String

(read)



## Index Parameters

* Index (Long)




## Description



Via this property you can output the actual entry id.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//get entry ids
EntryIDs oIds = oTb.Entries.GetEntryIDs();
for(int i=1;i==oIds.Count;i++)
{
   	Debug.WriteLine(oIds[i]);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.EntryIDs.Item)

