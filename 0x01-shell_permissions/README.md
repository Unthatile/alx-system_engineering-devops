#!/bin/bash
su betty = script that switches the current user to the user
whoami = script that prints the effective username of the current user
group = script that prints all the groups the current user is part of
sudo chown betty hello = script that changes the owner of the file hello to the user betty
touch hello = script that creates an empty file called hello
chmod u+x hello = script that adds execute permission to the owner of the file hello
chmod 754 = script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello
chmod 777 = script that adds execution permission to the owner, the group owner and the other users, to the file hello
