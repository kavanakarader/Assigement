$ git init
Initialized empty Git repository in C:/Users/Admin/Desktop/cdv0065/.git/

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git remote add origin "https://github.com/kavanakarader/Assigement.git"

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ notepad sample.text
/usr/bin/notepad: line 10: exec: notepad.exe: not found

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ notepad sample.txt
/usr/bin/notepad: line 10: exec: notepad.exe: not found

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ vi sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git add .
warning: in the working copy of 'sample.txt', LF will be replaced by CRLF the next time Git touches it

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git commit -m "first commit in feature branch"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Admin@DESKTOP-N872A1D.(none)')

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ ^C

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$  git config --global user.email "kavanask471@gmail.com"

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git config --global user.name "kavanakarader"

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git commit -m "first commit in feature branch"
[master (root-commit) e267771] first commit in feature branch
 1 file changed, 3 insertions(+)
 create mode 100644 sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 261 bytes | 130.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kavanakarader/Assigement.git
 * [new branch]      master -> master

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git branch feature-branch

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git checkout feature-branch
Switched to branch 'feature-branch'

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (feature-branch)
$ vi sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (feature-branch)
$ git add .
warning: in the working copy of 'sample.txt', LF will be replaced by CRLF the next time Git touches it

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (feature-branch)
$ git commit -m "first commit in feature-branch"
[feature-branch 4b1e343] first commit in feature-branch
 1 file changed, 2 insertions(+), 1 deletion(-)

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (feature-branch)
$ git push origin feature-branch
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 308 bytes | 154.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feature-branch' on GitHub by visiting:
remote:      https://github.com/kavanakarader/Assigement/pull/new/feature-branch
remote:
To https://github.com/kavanakarader/Assigement.git
 * [new branch]      feature-branch -> feature-branch

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (feature-branch)
$ git checkout master
Switched to branch 'master'

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git merge feature-branch
Updating e267771..4b1e343
Fast-forward
 sample.txt | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0065 (master)
$ git push origin master
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kavanakarader/Assigement.git
   e267771..4b1e343  master -> master
