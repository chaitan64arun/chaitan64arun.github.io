---
layout: post
title:  Configure GIT for multiple Users
tags:
- GIT
- Technology
---

I use Eclipse for Java development environment on Windows platform.
In this article, we will clone an existing Git repository.  

[In the complete article we are not using authentication details anywhere except adding the ssh key in github.com]

#### Step 1: Download Eclipse and install Eclipse.
Can be downloaded for www.eclipse.org. Extract the file and run eclipse.exe
A copy of shortcut on the desktop is recommended for easy navigation.

#### Step 2: Install EGit for Eclipse.

* Help-> Install New Software
* Put http://download.eclipse.org/egit/updates and Add
* Select Git from the drop down and Install
* Accept all licence terms and etc.

#### Step 3: Add SSH key.

Navigate to
> Windows-> Preferences-> general -> Network Connections -> SSH2

* Choose Key Management Generate a DSA key..
* Choose pass phrase if you want.
* Save the private key (.ssh folder by default)
* Copy the public key to the clipboard (important)

#### Step 4: Add the public key to Dashboard

This clipboard can be added to the SSH keys in the dash board of github.com

> Account Settings (on the top right) -> SSHkeys

#### Step 5: Import Git Repository

> File -> Import -> Git -> Projects from Git(from the cascaded tree) -> Next

Select URI

* You should choose the appropriate repository
> [eg: git@github.com:chaitan64arun/GitRepo.git]

* Choose protocol as SSH
* Select a valid branch [eg: Master]
* Choose Directory and remote name
* Wait for project to be Cloned

You get an another window, choose appropriately.
Then it s done..!!

### Different for different users

#### Step 6: Open project from Eclipse.

Use Team Synchronizing Perspective to easily commit changes and push it to the remote repository

Done…!! Now more than one developer can work on a project.

P.S. By adding the SSH key, you are allowing the user to modify your other repositories as well.
