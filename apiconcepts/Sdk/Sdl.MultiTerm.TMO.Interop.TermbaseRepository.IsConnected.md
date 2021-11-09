

# 
    IsConnected property



## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.IsConnected —          Indicates whether a connection has been established successfully.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



This property returns True or False depending on whether a connection to a termbase server has been established successfully or not.

You can use this property to ascertain whether the login was successful and output a corresponding message if this is not the case.



## Sample


```cs
if(oServRep.IsConnected)
{
   	MessageBox.Show("Login successful");
} 
else 
{
   	MessageBox.Show("Login failed.");
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.TermbaseRepository.IsConnected)

