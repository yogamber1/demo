its a read me file
branches
1. master 
2. feature
3. direct
 // merged with feature
 
 
commands used for reference


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep
$ git version
git version 2.31.1.windows.1

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep
$ git init
Initialized empty Git repository in C:/Users/yogamber singh negi/Desktop/new rep/.git/

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ touch new.html

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git add new.html

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   new.html


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git commit -m "first commit"
[master (root-commit) 9b12783] first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.html

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git checkout -b feature
Switched to a new branch 'feature'

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ touch text.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git add .

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git status
On branch feature
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   text.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git commit -m "commit on feature"
[feature 7073ec3] commit on feature
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 text.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git checkout -b direct
Switched to a new branch 'direct'

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ touch temp.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git add temp.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git status
On branch direct
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git status
On branch direct
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git remote add origin https://github.com/yogamber1/demo.git

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 211 bytes | 52.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/yogamber1/demo.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git push -u origin feature
gEnumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 246 bytes | 123.00 KiB/s, done.
remote: (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'feature' on GitHub by visiting:
remote:      https://github.com/yogamber1/demo/pull/new/feature
remote:
To https://github.com/yogamber1/demo.git
 * [new branch]      feature -> feature
Branch 'feature' set up to track remote branch 'feature' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git push -u origin direct
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'direct' on GitHub by visiting:
remote:      https://github.com/yogamber1/demo/pull/new/direct
remote:
To https://github.com/yogamber1/demo.git
 * [new branch]      direct -> direct
Branch 'direct' set up to track remote branch 'direct' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git status
On branch direct
Your branch is up to date with 'origin/direct'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git status
On branch direct
Your branch is up to date with 'origin/direct'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   text.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git add text.txt
warning: CRLF will be replaced by LF in text.txt.
The file will have its original line endings in your working directory

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git checkout feature
Switched to branch 'feature'
A       temp.txt
M       text.txt
Your branch is up to date with 'origin/feature'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git status
On branch feature
Your branch is up to date with 'origin/feature'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt
        modified:   text.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git push -u origin feature
Everything up-to-date
Branch 'feature' set up to track remote branch 'feature' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git merege direct
git: 'merege' is not a git command. See 'git --help'.

The most similar command is
        merge

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git merge direct
Already up to date.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git checkout direct
Switched to branch 'direct'
A       temp.txt
M       text.txt
Your branch is up to date with 'origin/direct'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git push -u origin direct
Everything up-to-date
Branch 'direct' set up to track remote branch 'direct' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git status
On branch direct
Your branch is up to date with 'origin/direct'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   temp.txt
        modified:   text.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   text.txt


player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git add text.txt
warning: CRLF will be replaced by LF in text.txt.
The file will have its original line endings in your working directory

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git commit
Aborting commit due to empty commit message.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git commit -m "commit modified"
[direct c17c472] commit modified
 2 files changed, 3 insertions(+)
 create mode 100644 temp.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git push -u origin direct
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 300 bytes | 100.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/yogamber1/demo.git
   7073ec3..c17c472  direct -> direct
Branch 'direct' set up to track remote branch 'direct' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git checkout direct
Already on 'direct'
Your branch is up to date with 'origin/direct'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (direct)
$ git checkout feature
Switched to branch 'feature'
Your branch is up to date with 'origin/feature'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git feature
git: 'feature' is not a git command. See 'git --help'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git status
On branch feature
Your branch is up to date with 'origin/feature'.

nothing to commit, working tree clean

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git merge direct
Updating 7073ec3..c17c472
Fast-forward
 temp.txt | 0
 text.txt | 3 +++
 2 files changed, 3 insertions(+)
 create mode 100644 temp.txt

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git commit -m "merge commit"
On branch feature
Your branch is ahead of 'origin/feature' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git push -u origin feature
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/yogamber1/demo.git
   7073ec3..c17c472  feature -> feature
Branch 'feature' set up to track remote branch 'feature' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (feature)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ touch README.md

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git add .

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git commit -m "readme created"
[master b419587] readme created
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 246 bytes | 82.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/yogamber1/demo.git
   9b12783..b419587  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git add .
warning: CRLF will be replaced by LF in README.md.
The file will have its original line endings in your working directory

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git push -u origin master
Everything up-to-date
Branch 'master' set up to track remote branch 'master' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git commit -m "read me "
[master 577d0bf] read me
 1 file changed, 6 insertions(+)

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ git push -u origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 343 bytes | 114.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/yogamber1/demo.git
   b419587..577d0bf  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

player x@DHINCHIKKIPC MINGW64 ~/Desktop/new rep (master)
$ 
