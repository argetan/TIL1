## 1. git 초기 설정

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice
$ git init
Initialized empty Git repository in C:/Users/limok/OneDrive/바탕 화면/practice/.git/

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ ls -a
./  ../  .git/

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ touch a.txt b.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git add a.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   a.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        b.txt


limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git commit -m "initial commit"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'limok@DESKTOP-B8A48SK.(none)')

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ ^C

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config ==global user.email "limokokpk2@gmail.com"
error: key does not contain a section: ==global

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config --global user.name "taesub"

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config --global --list
user.name=taesub

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ ^C

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config --global user.email "limokokpk2@gmail.com"

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config --global --list
user.name=taesub
user.email=limokokpk2@gmail.com

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git config --global core.editor "code --wait"

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git commit -m "initial commit"
[master (root-commit) e82e7a9] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git log
commit e82e7a9315b9683e969e6cd85c08678ba19bbcc1 (HEAD -> master)
Author: taesub <limokokpk2@gmail.com>
Date:   Mon Jul 5 15:25:32 2021 +0900

    initial commit

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git log --oneline
e82e7a9 (HEAD -> master) initial commit

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        b.txt

nothing added to commit but untracked files present (use "git add" to track)

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice (master)
$





실습

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1
$ git init
Initialized empty Git repository in C:/Users/limok/OneDrive/바탕 화면/practice1/.git/

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$ touch a.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$ git add a.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   a.txt


limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$ git commit -m "practice1 commit"
[master (root-commit) 40bfc5e] practice1 commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 a.txt

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$ git log
commit 40bfc5e30f2ad86447abfca8159019f2e92d8709 (HEAD -> master)
Author: taesub <limokokpk2@gmail.com>
Date:   Mon Jul 5 15:39:22 2021 +0900

    practice1 commit

limok@DESKTOP-B8A48SK MINGW64 ~/OneDrive/바탕 화면/practice1 (master)
$