su betty--script that changes your user ID to betty
id -un--prints the effective username of the current user
id -Gn--prints all the groups the current user is part of
chown betty hello--changes the owner of the file hello to the user betty
touch hello--create an empty file called hello
chmod u+x hello--add execute permission to the owner of the file hello
chmod ug+x,o+r hello--add execute permission to user and group owner and read permission to others to the file hello
chmod ugo+x hello--adds execution permission to all users to the file hello
chmod 007 hello--set permission to the file so that owner and group dont have any permission and other users have all permissions
chmod 753 hello--set permission so owner has all permissions, group has read and execute permissions and others have write and execute permissions
chmod --reference=olleh hello--copies the mode of the file olleh to the file hello
chmod -R +X .--add execute permission to all subdirectories of the current directory for everyone. Regular files should not be changed
mkdir -m 751 my_dir--create a directory called my_dir with permissions 751 in the working directory. User has all read, write and execute permissions, group has read and execute permissions and others have just execute permission
chgrp school hello--change group owner to school for the file owner
chown vincent:staff *--change owner to vincent and the group owner to staff for all the files and directories in the working directory
chown -h vincent:staff _hello--change the owner and group owner of hello to vincent and staff respectively
chown --from=guillaume betty hello--change owner of the file hello to betty if it is currently owned by guillaume
telnet towel.blinkenlights.nl--play the Star Wars IV episode in the terminal. This is a premade script provided online