
# Connecting to a MultiTerm Server

The first thing you need to do before you can access MultiTerm client functionality programmatically is to initiate a MultiTerm client object instance, i.e.:


```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
```

From the MultiTerm client object you can connect to two termbase repositories: a local and/or a remote (server) repository. Local termbases are stored as \*.sdltb files on the user's hard disk. Local termbase repositories do not require authentication. Nevertheless you need to apply the **Connect** method to the local repository and provide the user name and login. However, you may just provide two empty strings as login parameters, i.e.:


```cs
TermbaseRepository oLocalRep = oMt.LocalRepository;
oLocalRep.Connect("","");
Debug.WriteLine("Connection successful: " + oLocalRep.IsConnected);
```

Connecting to a remote, i.e. server repository requires you to enter a 'real' user name and password. In addition you need to specify the server name (location), e.g.:


```cs
Sdl.MultiTerm.TMO.Interop.Application oMt = new Sdl.MultiTerm.TMO.Interop.ApplicationClass();
TermbaseRepository oServerRep = oMt.ServerRepository;
oServerRep.Connect("guest","guest");
oServerRep.Location = "http://termserver";
Debug.WriteLine("Connection successful: " + oServerRep.IsConnected);
```




