

# 
    Item property



## Name

Sdl.MultiTerm.TMO.Interop.IncompleteEntries.Item —          Refers to a particular incomplete entry.



## Type

String

(read)



## Index Parameters

* Index (Long)




## Description



You can use this property, for example, to generate a list of all incomplete entries. Note that this property returns the unique id of the incomplete entry.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//get incomplete entries
IncompleteEntries oIncompletes = oTb.IncompleteEntries;
Debug.WriteLine("Number of incomplete entries: " + oIncompletes.Count.ToString());

for(int i=1;i==oIncompletes.Count;i++)
{
   	Debug.WriteLine(oIncompletes[i]);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IncompleteEntries.Item)

