
# Selecting a Termbase

Once you have connected to a termbase repository you can select one or more termbases. To refer to a specific termbase you can either use its index number or the actual (nice) name used to uniquely identify a termbase, e.g.:


```cs
Termbases oTbs = oServerRep.Termbases;
Termbase oTb = oTbs["Termbase name"];
```

From this point onwards you can perform further operations such as [searching](searching.htm) the termbase or accessing the termbase entries. The following line, for example, returns the total number of entries contained in a termbase:


```cs
Debug.WriteLine("Total number of entries in termbase: " + oTb.Entries.Count.ToString());
```

When implementing a MultiTerm client you will usually want to offer a termbase selection to the users, e.g. a list control filled with the respective termbase names. The sample code below lists the names of all termbases available in a repository:


```cs
Termbases oTbs = oServerRep.Termbases;
foreach (Termbase oTb in oTbs)
{
   Debug.WriteLine(oTb.Name);
}
```




