# Sdl.MultiTerm.TMO.Interop.MtUserType Enumeration

## Name

Sdl.MultiTerm.TMO.Interop.MtUserType —          The user privilege types used for termbase access.

## Description

Basically, there are two different types of users: 'normal' users, i.e. those who access termbases via MultiTerm client applications such as the MultiTerm iX LAN client, MultiTerm Online or the MultiTerm Word interface. Then, there are the 'super' users (or administrative users). These users are allowed to create and administer server termbases, create user roles, etc. dedicated client applications such as MultiTerm Administrator.

This enumerator contains the available user privilege type values.

## Values

* *mtNormalUser*

    Normal users with read and/or write access to termbases via clients such as the MultiTerm Workstation client or MultiTerm Online
* *mtNotAuthorized*

    Users without any access privileges.
* *mtSuper*

    Administrative user, who can create termbases, define user roles, etc. via MultiTerm Administrator.
