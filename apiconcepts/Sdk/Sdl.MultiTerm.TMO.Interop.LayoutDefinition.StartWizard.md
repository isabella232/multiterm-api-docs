

# 
    StartWizard method



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.StartWizard —          Calls up the layout definition wizard for editing a particular layout.



## Returntype

void



## Parameters

* XMLFileName (String, *optional*)




## Description



Applying this method to a layout definition, opens the layout definition wizard, which allows for GUI-based editing of the layout. This method takes the name and path of an external layout definition (\*.xdl) file as parameter. This means that you can provide an external layout definition file to 'pre-fill' the wizard with some information.

Note that the currently-logged in user needs to have permissions to edit the layout in question, otherwise an error will be thrown.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout=oLayouts["My own layout"];
oLayout.StartWizard("c:\\temp\\update_content.xdl");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinition.StartWizard)

