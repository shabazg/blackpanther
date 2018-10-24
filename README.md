# blackpanthergithubtraining
Its an application for Avengers
============================================



pwd
Path:
cd /c/Shabaz/Git

git clone https://github.com/praqma-training/git-katas.git
git clone https://github.com/shabazkhan033/blackpanther
git status
git log
for quit --- Hit  q
save and quit --- :wq!
==
echo "This Is My file" > myFile.txt
git add myFile.txt

git status
git commit -m "My First Commit!"
git status
===

===Issues===

$ git commit -m "My First Commit! KHAN"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'se34882@IBM830-R90LT6N7.(none)')

se34882@IBM830-R90LT6N7 MINGW64 /c/Shabaz/GITWorkspace/gitkatas (master)
$ git config --global user.email "shabaz.g@ikea.com"

se34882@IBM830-R90LT6N7 MINGW64 /c/Shabaz/GITWorkspace/gitkatas (master)
$ git config --global user.name "Shabaz"

====
Notepad on WIndows
git config --global core.editor notepad
===




Working Directoy - Staging Directory - Commit
Status:
1. Untrackeed
2. Unmodified
3. Modififed
4. Staged

Find Instructions in gitkatas/basic-commits

git add
git commit
git commit -m
git log
git log -n 5
git log --oneline
git log --oneline --decorate --graph
git log --decorate
git log --decorate --oneline --graph

touch filename to create a file
echo content > file to overwrite file with content
echo content >> file to append file with content

git diff (Compare local to staged area)
nano <File Name> - shows the differences

git diff --staged (Compare all the changes added which to commit will compare with Master)
git diff --


=====Staging======
git checkout file.txt  ?????


===
Ignoring files
*.log
*.ssh
biild/

Add a .gitignore file in the work tree or a sub folder

touch (to create file)
.gitignore file ??


==
Time to customize
Aliases
You can set up aliases as such: git config --global alias.lol 'log --oneline --decorate --graph --all' This might be useful to you.

#simple alias for git checkout
git config --global alias.co "checkout"


git config -l 
git config -l --show-origin



git
Directed Acyclical Graph (DAG)

collection of object and reference to these object

GIT object
compression of files and make it as object which has reference
Objects are immutable

4 types of objetc
blob (file content) -
tree  - flat file ... list of blobs. its like folder
commit - points to tree (root) ...stores info: author, commit message and tree . it can have many parents (Merge from A to B)
tag - Annoted Tag


Objetcs are stored in : <>


/c/Shabaz/GITWorkspace/gitkatas/.git 

git cat -file -p .git/object/......

git show master  (what info on any object)
git show 



se34882@IBM830-R90LT6N7 MINGW64 /c/Shabaz/GITWorkspace/gitkatas/.git/objects (GIT_DIR!)
$ ls 21
4bea0230aa7b0660163a765889244d3386b799

se34882@IBM830-R90LT6N7 MINGW64 /c/Shabaz/GITWorkspace/gitkatas/.git/objects (GIT_DIR!)
$ git cat-file -p 214bea0230aa7b0660163a765889244d3386b799



===== investigation===========



====================Own Respository===========
git init


=== Branching===
branch is pointer to commit.

git branch 
HEAD is points to Master
uppercase

checkout will point HEAD to master... always


commands:
git branch
git checkout <<branch name>>
git branch -v

git diff branch1 branch2

==== Refs====
.git/refs/ folder
types of refs:
branches
remotes
lightweight tag

HEAD -points to current branch


print content of file 
\cat master 

head -> branch -> Commit -> tree -> blod


==Merging===
git checkout master
git merge uppercase

deleting the branch
git branch -d uppercase
==

reset
git reset <tree-ish>

reset types:
soft
mixed
hard

git reset --soft <tree-ish>

git clean
delete untrackeed files

git clean --dry-run


git remote -v
git remote add <name> <url>
git remote rm <name>

git fetch <remote>
git fetch <remote> <branch>


git pull <remote>  ---- fetch and merge

git push <remote> <branch>
git push <remote> <local-branch>:<remote-branch>
git push <remote> -all (push all branches)
git push <remote> --tags (push all tags)
git push <remote> --delete <branch>
  
  
  =============================
