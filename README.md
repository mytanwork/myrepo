2018-06-30 Play around with git and github

new line input from shell


git remote show origin ## show whether the repo is remote or local
* remote origin
  Fetch URL: https://github.com/mytanwork/myrepo.git
  Push  URL: https://github.com/mytanwork/myrepo.git
  HEAD branch: (unknown)
  Local branch configured for 'git pull':
    master merges with remote master


admins-MacBook-Pro:myrepo mengyao$ cat > README.md
2018-06-30 Play around with git and github


admins-MacBook-Pro:myrepo mengyao$ echo "new line input from shell" >> README.md 

admins-MacBook-Pro:myrepo mengyao$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md

nothing added to commit but untracked files present (use "git add" to track)


admins-MacBook-Pro:myrepo mengyao$ git add -A


admins-MacBook-Pro:myrepo mengyao$ git commit -m "A commit from my local computer"
[master (root-commit) 6289e2a] A commit from my local computer
 1 file changed, 2 insertions(+)
 create mode 100644 README.md
 
 
admins-MacBook-Pro:myrepo mengyao$ git push
Username for 'https://github.com': mytanwork@gmail.com
Password for 'https://mytanwork@gmail.com@github.com': 
Counting objects: 3, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 295 bytes | 295.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/mytanwork/myrepo.git
 * [new branch]      master -> master
 
 

admins-MacBook-Pro:myrepo mengyao$ git branch -vv
* master 6289e2a [origin/master] A commit from my local computer


admins-MacBook-Pro:myrepo mengyao$ git --version
git version 2.15.2 (Apple Git-101.1)


admins-MacBook-Pro:myrepo mengyao$ git credential-osxkeychain
usage: git credential-osxkeychain <get|store|erase>
admins-MacBook-Pro:myrepo mengyao$ ls -al ~/.ssh
total 8
drwx------   3 mengyao  staff    96 Jan 10 09:35 .
drwxr-xr-x+ 35 mengyao  staff  1120 Jun 30 15:38 ..
-rw-r--r--   1 mengyao  staff   533 Feb 22 15:56 known_hosts

admins-MacBook-Pro:myrepo mengyao$ sudo vim /etc/hosts
Password:
