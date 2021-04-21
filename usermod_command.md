## ```usermod``` command
- shows version : 
- show help page : usermod --help
- add a piece of information about a user : sudo usermod -c "Good Morning" test_user (sudo usermod -c "information" username)
- to change the location of the user’s home folder : sudo usermod -d /home/test_user test_user (sudo usermod -d directory-location username) 
- to change the location of the user’s home folder and move the content of the user’s home directory : sudo usermod -d /home/test_user -m test_user (sudo usermod -d location -m username)
- setting up a user account expiry date : sudo usermod -e 2021-04-22 test_user (sudo usermod -e YYYY-MM-DD username)
- to change the default shell for a single user : sudo usermod -s /bin/bash test_user (sudo usermod -s shell username)
- to change user UID : sudo usermod -u 7321 test_user (sudo usermod -u new-UID username)
- to change user login name : sudo usermod -l new_name test_user (sudo usermod -l newname oldname)
- to lock a user account : sudo usermod -L user (sudo usermod -L username)
- to unlocak a user account : sudo usermod -U user (sudo usermod -U username)
- to set a un-encrypted password for a user : sudo usermod -p abc123 user (sudo usermod -p password username)
- to change the primary group of a user : sudo usermod -g new_group user (sudo usermod -g group username)
- to add a user in supplementary groups : sudo usermod -G root user (sudo usermod -G group username)
 - to add the user to the specified group and leave them in the supplementary group they were already a member of : sudo usermod -a -G test_group user (sudo usermod -a -G group username)
 
 
 
 
 ## tips:
- sudo usermod -d home-folder -s shell -e YYYY-MM-DD -c "comment" -u UID -aG group username
