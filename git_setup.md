# Git Set-Up

## 1. Linking A New Repo 
Open new bash terminal. 
```
mkdir pets_lost_and_found
cd pets_lost_and_found/
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
**Remote origin should be same url as repo. However, if different...**
```
git remote remove origin 
git remote add origin [repo https url].
```
Otherwise, contine from the `cat .git/config`. 


