# python_code
spam boiiii

commands used till now:
cmd to check if process is running: eval "$(ssh-agent -s)"
connecting git to github and autheticating device
1.key generation
cmd: ssh-keygen [ -tb rsa 4096] (optional to specify the algorithm but works with ssh-keygen too)
2.Generated public and private keys, copy public key to github(setting-->ssh bla bla--> new ssh key)
3.Copy private key to ssh-agent by following command:
cmd: ssh-add ~/.ssh/id_rsa     (id_rsa is the file name generated after running keygen cmd for priv key)  //.pub is public key
4. set global variables:
cmd: global

local to server:
server to local:
1. git clone <repository_name>	(copied from github ssh||https)
//
1. git status
2. git add . //(all)
3. git commit -m <message>//(commits changes to tracking)
4. git push //(commits changes to server/local system)

