# Git Set-Up

## 1. Linking A New Repo 
Open new bash terminal. 
```
mkdir my_memos
cd my_memos
git init
ls -a
```
Make a read me. `code .` will open up a coding platform such as VS Code. 
```
touch README.md
code . 
```
Make changes to the `README` file. 
```
git add .
git status
git commit -m "initial commit"
git config --global user.email "email@address.com"
git config --global user.user "michelle"
```
Make a new repository in github and link using given https link.
```
git remote add origin https://github.com/MichelleHM/my_memos.git
git push 
git push --set-upstream origin master 
```
## 2. Checking if github is linked. 
Following on from same terminal, in the same directory where `README` is saved. 
```
cat .git/config
```
The remote origin should be a https. Now, we are changing the connection to SSH. SSH link will be in the github repo. 
```
git remote remove origin 
git remote add origin git@github.com:MichelleHM/my_memos.git
```
## 3. Allowing auto authentication when git push

This step will only need to be done once for your current computer. A new key will be needed for additional devices. 
```
cd ~ 
cd .ssh
ssh-keygen 
cat ~/.ssh/id_rsa.pub

```
Copy the entire key and then login into your Github account. 

```
Github > Settings > SSH and GPG keys > New SSH Key. 
```

Paste the key into the provided space. 

Now your computer is linked to your github!
asdf finally figured out how to do more

