#!/bin/bash

su betty = script that switches the current user to the user

whoami = script that prints the effective username of the current user

group = script that prints all the groups the current user is part of

sudo chown betty hello = script that changes the owner of the file hello to the user betty

touch hello = script that creates an empty file called hello

chmod u+x hello = script that adds execute permission to the owner of the file hello

chmod 754 = script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello

chmod ugo+x = script that adds execution permission to the owner, the group owner and the other users, to the file hello

chmod 007 = script that sets the permission to the file hello as follows:

									Owner: no permission at all
									Group: no permission at all
									Other users: all the permission

chmod 753 hello = script that sets the mode of the file hello to this:

									-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
									The file hello will be in the working directory
