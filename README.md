# python_code
spam boiiii

commands used till now:

cmd to check if process is running: eval "$(ssh-agent -s)"
cmd to check if ssh connection is established: ssh -T git@github.com
connecting git to github and autheticating device+
1.key generation
cmd: ssh-keygen [ -tb rsa 4096] (optional to specify the algorithm but works with ssh-keygen too)
2.Generated public and private keys, copy public key to github(setting-->ssh bla bla--> new ssh key)
3.Copy private key to ssh-agent by following command:
cmd: ssh-add ~/.ssh/id_rsa     (id_rsa is the file name generated after running keygen cmd for priv key)  //.pub is public key
4. set global variables for username and email:
cmd: git config --global user.email "s.ashutosh4490@gmail.com" 
cmd: git config --global user.name "fornclakess"
5.(optional) if not on main brach, cmd to rename local branch(i.e. master) to match that of github's(main)
cmd: git branch -m master main


local to server:
1. create a folder named "itna lodu kyu ha tu kishan"
2. open bash inside
3. git init (for initialisation of folder as git repo)
4. git status
5. git remote add origin <ssh/https link>
to remove: git remote remove origin
6. git remote -v (to check if and where it's connected for fetch and push)
7. repeat regular steps(status,add,commit,push)



server to local:
1. git clone <repository_name>	(copied from github ssh||https)
1. git status
2. git add . //(all)
3. git commit -m <message>//(commits changes to tracking)
4. git push //(commits changes to server/local system)

//local ------> server on branch main
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin <ssh link>
git push -u origin main
 
