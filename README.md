# ansible-jenkins-gerrit-transmission

Here is a playbook for Ubuntu 14.04 that installs Jenkins and Gerrit using war file and Transmission daemon 
via apt. 

Three application accounts are created with approriate names and three developer accounts with names devel1, devel2 and devel3 are added. All application settings are stored in home directories. 
All three applications are placed in Firejail sandbox (https://firejail.wordpress.com/) and don't have access to file system. To run this playbook, the following command should be run after cloning: 

*ansible-playbook site.yml --ask-sudo-pass*
