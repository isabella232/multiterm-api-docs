#  ChangePassword method


## Name

Sdl.MultiTerm.TMO.Interop.TermbaseRepository.ChangePassword —          Changes the password of the currently logged-in user.

## Returntype

void

## Parameters

* NewPassword (String)
* OldPassword (String, *optional*)


## Description

Applying this method will change the password for the currently logged-in user. It requires the old password and the new password as string parameters.

You would use this method if you wanted to implement a function in your client application that allows users to change their password themselves rather than having to contact the MultiTerm administrator to do this for them. Passwords are stored in the database backend in encrypted format.

## Sample


```cs
oServRep.Connect("username", "oldpassword");
oServRep.ChangePassword("oldpassword", "newpassword");
```

