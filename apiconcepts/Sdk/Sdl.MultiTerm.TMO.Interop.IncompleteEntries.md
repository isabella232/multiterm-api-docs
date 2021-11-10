

# 
    Sdl.MultiTerm.TMO.Interop.IncompleteEntries class




## Name

Sdl.MultiTerm.TMO.Interop.IncompleteEntries —          Provides access to all incomplete entries of a termbase.



## Description



Incomplete entries are entries that lack one or more fields that are mandatory according to the termbase definition. For example, if the termbase definition imposes that the field "Subject" is mandatory and an entry does not have a "Subject" field, it is considered incomplete. In this case the corresponding XML data stored in the mtConcepts table of the database backend will be marked as incomplete, i.e. it will have the value '1' in the 'incomplete' column.
.md)
When adding a new entry programmatically via the [New](Sdl.MultiTerm.TMO.Interop.Entries.New.md) method, you can flag it as incomplete by setting the incomplete parameter to true.

This is, for example, the case for all entries that are added via the Quick Entry function from Word. Note that your client needs to implement the logic that decides whether an entry is incomplete or not. This is not done on the server side.

You can use the IncompleteEntries class, for example, to compile a list of all termbase entries that are flagged as incomplete, which can be useful for maintenance purposes. Thus you can implement a feature similar to the Incomplete Search in MultiTerm Workstation.



## Properties

* [Count](Sdl.MultiTerm.TMO.Interop.IncompleteEntries.Count.md): Returns the number of incomplete entries contained in a termbase.
* [Item](Sdl.MultiTerm.TMO.Interop.IncompleteEntries.Item.md): Refers to a particular incomplete entry.




## Methods
*None*


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

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.IncompleteEntries)

