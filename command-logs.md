khair_ubunt@KHAIRUL-Hp:~$ ls
devops-task-1  health.sh  hello.txt  link-practise  newfile.sh  permission  text.txt  zip-practise
khair_ubunt@KHAIRUL-Hp:~$ mkdir devops-task-2
khair_ubunt@KHAIRUL-Hp:~$ cd devops-task-2
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git --version
git version 2.43.0
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ sudo apt update
[sudo] password for khair_ubunt:
Get:1 http://security.ubuntu.com/ubuntu noble-security InRelease [126 kB]
Hit:2 http://archive.ubuntu.com/ubuntu noble InRelease
Get:3 http://archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]
Get:4 http://security.ubuntu.com/ubuntu noble-security/main amd64 Components [21.5 kB]
Get:5 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Components [71.4 kB]
Get:6 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Components [212 B]
Get:7 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Components [212 B]
Get:8 http://archive.ubuntu.com/ubuntu noble-backports InRelease [126 kB]
Get:9 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [1694 kB]
Get:10 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Components [175 kB]
Get:11 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 Packages [1512 kB]
Get:12 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 Components [377 kB]
Get:13 http://archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Components [212 B]
Get:14 http://archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Components [940 B]
Get:15 http://archive.ubuntu.com/ubuntu noble-backports/main amd64 Components [7304 B]
Get:16 http://archive.ubuntu.com/ubuntu noble-backports/universe amd64 Components [10.5 kB]
Get:17 http://archive.ubuntu.com/ubuntu noble-backports/restricted amd64 Components [216 B]
Get:18 http://archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 Components [212 B]
Fetched 4249 kB in 13s (339 kB/s)
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
7 packages can be upgraded. Run 'apt list --upgradable' to see them.
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ sudo apt install git
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
git is already the newest version (1:2.43.0-1ubuntu7.3).
git set to manually installed.
0 upgraded, 0 newly installed, 0 to remove and 7 not upgraded.
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git --version
git version 2.43.0
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git config --global --list
fatal: unable to read config file '/home/khair_ubunt/.gitconfig': No such file or directory
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git config --global user.name "Khairul Islam"
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git config --global user.email "ki733655@gmail.com"
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git config --global --list
user.name=Khairul Islam
user.email=ki733655@gmail.com
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls -l
total 0
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in /home/khair_ubunt/devops-task-2/.git/
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls -l
total 0
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls -a
.  ..  .git
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ touch file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls
file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ vim file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ cat file.txt
It is the text file
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file.txt

nothing added to commit but untracked files present (use "git add" to track)
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git add file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git commit -m "My first commit"
[master (root-commit) e483c58] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git status
On branch master
nothing to commit, working tree clean
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git branch
* master
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git branch -M main
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git branch
* main
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git remote add origin https://github.com/ki733655/devops-task-2.git
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655@gmail.com
Password for 'https://ki733655%40gmail.com@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655@gmail.com
Password for 'https://ki733655%40gmail.com@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git remote add origin https://github.com/ki733655/devops-task-2.git
git branch -M main
git push -u origin main
error: remote origin already exists.
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push -u origin main
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 237 bytes | 237.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ki733655/devops-task-2.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git check
git: 'check' is not a git command. See 'git --help'.

The most similar command is
        checkout
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git checkout -b feature
Switched to a new branch 'feature'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ ls
file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ nano file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ cat file.txt
It is the text file
now its edited for the feature branch
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git add file.txt
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git commit -m "Updated file"
[feature ea90155] Updated file
 1 file changed, 1 insertion(+)
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git status
On branch feature
nothing to commit, working tree clean
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git branches
git: 'branches' is not a git command. See 'git --help'.
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git git merge feature
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git merge feature
Updating e483c58..ea90155
Fast-forward
 file.txt | 1 +
 1 file changed, 1 insertion(+)
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push
Username for 'https://github.com': ki733655@gmail.com
Password for 'https://ki733655%40gmail.com@github.com':
remote: Invalid username or token. Password authentication is not supported for Git operations.
fatal: Authentication failed for 'https://github.com/ki733655/devops-task-2.git/'
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git push
Username for 'https://github.com': ki733655
Password for 'https://ki733655@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 298 bytes | 298.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ki733655/devops-task-2.git
   e483c58..ea90155  main -> main
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git log --oneline
ea90155 (HEAD -> main, origin/main, feature) Updated file
e483c58 My first commit
khair_ubunt@KHAIRUL-Hp:~/devops-task-2$ git log
commit ea9015572d3639ef56601ce0bcac9e1683053ccc (HEAD -> main, origin/main, feature)
Author: Khairul Islam <ki733655@gmail.com>
Date:   Fri Jan 16 14:17:29 2026 +0000

    Updated file

commit e483c5837bcab572101f52bdc72ea94c5641d2a7
Author: Khairul Islam <ki733655@gmail.com>
Date:   Fri Jan 16 13:51:28 2026 +0000

    My first commit
