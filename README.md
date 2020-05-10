# GIT-Everything
GIT-Everything


## I. Basic Command

### 1. List all configuration:
``` git config --list ```

### 2. Create a local branch:
``` git checkout -b branch_name```


### 3. Create ssh key - Add public key to GIT Sever
We will be able to work with git server via: `HTTPS` or `SSH` mode. Use HTTPS mode we will have to input the credential while we pull or push code to GIT server.
When add public key of our computer / workstation to GIT server, then we can work and contact to GIT server.

To create ssh key

``` ssh-keygen ```

### 4.Git Change 
```
git add . 
# or git
git add <fileName>
git status
git diff
git diff --staged
git reset <fileName>
git commit -am "Message Commit"
```

### 5. git add ssh key
`ssh-add -K ~/.ssh/doai_rsa`

## II. Git Branching Model
Github
GitLab
Gitbucket

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


