# GIT-Everything
GIT-Everything


## I. Basic Command

### List all configuration:
``` git config --list ```

### Create a local branch:
``` git checkout -b branch_name```


### Create ssh key
``` ssh-keygen ```

### Git Change 
```
git add . 
# or git
git add <fileName>
git status
git diff
git 

```


## II. Issues:

### 1. Reset everything to the lasted commit:

``` git reset --hard ```


### 2. Add one more account to git

```git config --list```
```
# Personal account, - the default config
Host github.com
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_rsa
# Work account-1
Host github.com-work_user1    
   HostName github.com
   User git
   IdentityFile ~/.ssh/id_rsa_work_user1
```   
Create one more ssh key with command: 


Reference:
https://medium.freecodecamp.org/manage-multiple-github-accounts-the-ssh-way-2dadc30ccaca


### 3. Error: Auto packing the repository in background for optimum performance. See "git help gc" for manual housekeeping.


Run this command: 
```git gc --prune=now```


