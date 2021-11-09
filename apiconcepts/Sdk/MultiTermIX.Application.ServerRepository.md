

# 
    ServerRepository property



## Name

MultiTermIX.Application.ServerRepository —          Provides access to the termbases stored on a MultiTerm Server.



## Type

[MultiTermIX.TermbaseRepository](MultiTermIX.TermbaseRepository.html)

(read)



## Index Parameters
*none*


## Description



Via this class you can access those termbases stored on a MultiTerm Server machine that your login allows you to access.

In order to access a MultiTerm Server you need to provide the server machine name and your user name and password.



## Sample


```cs
MultiTermIX.Application oMt = new MultiTermIX.ApplicationClass();
TermbaseRepository oServRep = oMt.ServerRepository;
oServRep.Location = "http://localhost";
oServRep.Connect("guest", "guest");
MessageBox.Show ("Server termbase count: " + oServRep.Termbases.Count.ToString());

oServRep.Disconnect();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20MultiTermIX.Application.ServerRepository)

