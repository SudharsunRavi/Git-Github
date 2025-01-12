## Git commands
```
git init
```
This is initialize git folder into the project directory

```
git status
```
This to see what are the files changes that are staged or has to be staged for commiting

```
git add .
git add filename.ext
git add file1.js file2.txt
```
This is to add the files to staged changes to commit to the repo. The dot adds every file to the repo

```
git restore --staged file1.txt
```
This is to unstage the staged change. Changes will be still there

```
git commit -m "message"
```
This is to commit the changes in staged

```
git log
```
Can checkc logs to the repo

```
git reset hash
```
This will go back to that specific commit and all the commits after this will be in unstaged area

```
git stash
```
Stash is basically u dont have to commit the stages now but save it somewhere so u can retrieve and use it.
Add the things that u wanna put it in the stash first then use git stash so everything in the staged will be stashed

```
git stash pop
```
This will bring back the code from stash space to the staged changes 

```
git stash clear
```
Deletes every file/changes in stash

## Linking git and github

```
git remote add origin https://github.com/SudharsunRavi/Git-Github.git
```
Link will be the same as clone one

```
git push origin branchName
```
Pushing the code to the particular branch, for main branch use "master" as the name

```
git branch branchName
```
Creates a new branch

```
git checkout branchName
```
Head points to that particular branch

```
git merge branchName
```
Will merge the branch to main

```
git clone <link>
git remote add upstream <parentRepoLink>
```
upstream will make sure the changes u make in ur repo will be asked to reflec tin parent repo

```
git pull upstream main
```

Fetches and pulls the latest update in parent repo

```
git rebase -i hash
```
The commits after the given hash will be shown like this
- pick hash1
- pick hash2
- pick hash3
- pick hash4

Change that to
- pic hash1
- s hash2
- s hash3
- s hash4

s refers to squash, here hash2,3,4 will be merged into hash1 making it as a single commit
