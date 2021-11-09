

# 
    StartWizard method



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.StartWizard —          Calls up the filter wizard for editing a particular filter.



## Returntype

void



## Parameters

* XMLFileName (String, *optional*)




## Description



Applying this method to a filter  definition, opens the filter wizard, which allows for GUI-based editing of the filter. This method takes the name and path of an external filter definition (\*.xdf) file as parameter. This means that you can provide an external filter definition file to 'pre-fill' the wizard with some information.

Note that the currently-logged in user needs to have permissions to edit the filter in question, otherwise an error will be thrown.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter = oFilters["Missing target"];
oFilter.StartWizard("c:\\temp\\filter.xdf");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.StartWizard)

