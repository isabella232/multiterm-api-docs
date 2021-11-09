

# 
    Save method



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Save —          Saves the selected termbase definition to an external file.



## Returntype

void



## Parameters

* FileName (String)




## Description



Applying this method to a TermbaseDefinition object saves the definition of the currently selected termbase to an external (\*.xdt) file.

The \*.xdt file can then be used as a template to create another termbase.

This method requires the full name and path of the external definition file as string parameters.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

TermbaseDefinition tbDef = oTb.Definition;
tbDef.Save("c:\\temp\\tb_def.xdt");
Debug.Write("Termbase definition saved successfully.");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseDefinition.Save)

