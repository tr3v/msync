msync
=====

A simple self-contained python script that leverage's rsync to maintain a synchronised directory on multiple computers:

This Python script will use various rsync commands to keep a selected local directoy syncronised with a remote server via SSH.
The syncronisation is two way and can support multiple clients to one server (think dropbox), so delted files/directorys will be reflected locally and on the server when the script is run. File conflicts are handled by the most recently modified
The server requires no special deamon process other than SSH however for the sake of smoothness a key-pair relationship is needed  with the server however the script includes a wizard to assist with this when using the --config-gen switch. 
