seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-1
error: pathspec '15-4-feature-1' did not match any file(s) known to git
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout -b 15-4-feature-1
Switched to a new branch '15-4-feature-1'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout -b 15-4-feature-2
Switched to a new branch '15-4-feature-2'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout -b 15-4-feature-3
Switched to a new branch '15-4-feature-3'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-2
Switched to branch '15-4-feature-2'
seirena1377@DESKTOP-7PMN61Q:~/test1$ ls -la
total 44
drwxr-xr-x 3 seirena1377 seirena1377 4096 Sep 22 22:22  .
drwxr-xr-x 6 seirena1377 seirena1377 4096 Sep 22 01:18  ..
drwxr-xr-x 8 seirena1377 seirena1377 4096 Sep 26 22:41  .git
-rw-r--r-- 1 seirena1377 seirena1377    6 Sep 22 22:11  12345
-rw-r--r-- 1 seirena1377 seirena1377   64 Sep 22 22:21  789.txt
-rw-r--r-- 1 seirena1377 seirena1377  742 Sep 22 22:22  INFO.md
-rw-r--r-- 1 seirena1377 seirena1377   87 Sep 16 23:49  README.md
-rw-r--r-- 1 seirena1377 seirena1377 1395 Sep 22 22:11  file-feature-2.txt
-rw-r--r-- 1 seirena1377 seirena1377 2438 Sep 22 22:11  file-main-feature.txt
-rw-r--r-- 1 seirena1377 seirena1377 6106 Sep 16 23:49 'Дом питомца.xlsx'
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano INFO.md
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano README.md
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano file-feature-2.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano  file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-3
M       file-main-feature.txt
Switched to branch '15-4-feature-3'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-2
M       file-main-feature.txt
Switched to branch '15-4-feature-2'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git add .
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-3
M       file-main-feature.txt
Switched to branch '15-4-feature-3'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-2
M       file-main-feature.txt
Switched to branch '15-4-feature-2'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git commit
[15-4-feature-2 d20105d] Удалила второй абзац, изменила третий абзац
 1 file changed, 1 insertion(+), 3 deletions(-)
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-3
Switched to branch '15-4-feature-3'
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano  file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ git commit -am "изменения в четвертом абзаце"
[15-4-feature-3 1c0901d] изменения в четвертом абзаце
 1 file changed, 1 insertion(+), 1 deletion(-)
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano  file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ git commit -am "удалила первый абзац и изменила второй"[master 9fb0c04] удалила первый абзац и изменила второй
 1 file changed, 1 insertion(+), 2 deletions(-)
seirena1377@DESKTOP-7PMN61Q:~/test1$ git pull origin master
From https://github.com/Seirena/test1
 * branch            master     -> FETCH_HEAD
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin master
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Seirena/test1.git
   4f3d95e..9fb0c04  master -> master
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-1
Switched to branch '15-4-feature-1'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git pull origin 15-4-feature-1
fatal: couldn't find remote ref 15-4-feature-1
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin 15-4-feature-1
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Total 0 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for '15-4-feature-1' on GitHub by visiting:
remote:      https://github.com/Seirena/test1/pull/new/15-4-feature-1
remote:
To https://github.com/Seirena/test1.git
 * [new branch]      15-4-feature-1 -> 15-4-feature-1
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin 15-4-feature-2
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 349 bytes | 349.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for '15-4-feature-2' on GitHub by visiting:
remote:      https://github.com/Seirena/test1/pull/new/15-4-feature-2
remote:
To https://github.com/Seirena/test1.git
 * [new branch]      15-4-feature-2 -> 15-4-feature-2
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin 15-4-feature-3
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 337 bytes | 337.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for '15-4-feature-3' on GitHub by visiting:
remote:      https://github.com/Seirena/test1/pull/new/15-4-feature-3
remote:
To https://github.com/Seirena/test1.git
 * [new branch]      15-4-feature-3 -> 15-4-feature-3
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-2
Auto-merging file-main-feature.txt
CONFLICT (content): Merge conflict in file-main-feature.txt
Automatic merge failed; fix conflicts and then commit the result.
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge --continue
U       file-main-feature.txt
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git add .
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge --continue
[master 9fa0506] Merge branch '15-4-feature-2'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-3
Auto-merging file-main-feature.txt
Merge made by the 'recursive' strategy.
 file-main-feature.txt | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano file-main-feature.txt
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git pull origin master
From https://github.com/Seirena/test1
 * branch            master     -> FETCH_HEAD
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin master
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
fatal: Authentication failed for 'https://github.com/Seirena/test1.git/'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin master
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 625 bytes | 625.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/Seirena/test1.git
   9fb0c04..34c6ae2  master -> master
seirena1377@DESKTOP-7PMN61Q:~/test1$ git sta
stage    stash    status
seirena1377@DESKTOP-7PMN61Q:~/test1$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
seirena1377@DESKTOP-7PMN61Q:~/test1$ is -la
is: command not found
seirena1377@DESKTOP-7PMN61Q:~/test1$ ls -la
total 44
drwxr-xr-x 3 seirena1377 seirena1377 4096 Sep 26 23:07  .
drwxr-xr-x 6 seirena1377 seirena1377 4096 Sep 22 01:18  ..
drwxr-xr-x 8 seirena1377 seirena1377 4096 Sep 26 23:18  .git
-rw-r--r-- 1 seirena1377 seirena1377    6 Sep 22 22:11  12345
-rw-r--r-- 1 seirena1377 seirena1377   64 Sep 22 22:21  789.txt
-rw-r--r-- 1 seirena1377 seirena1377  742 Sep 22 22:22  INFO.md
-rw-r--r-- 1 seirena1377 seirena1377   87 Sep 16 23:49  README.md
-rw-r--r-- 1 seirena1377 seirena1377 1395 Sep 22 22:11  file-feature-2.txt
-rw-r--r-- 1 seirena1377 seirena1377 2468 Sep 26 23:02  file-main-feature.txt
-rw-r--r-- 1 seirena1377 seirena1377 6106 Sep 16 23:49 'Дом питомца.xlsx'
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano 12345
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ delete 1235
delete: command not found
seirena1377@DESKTOP-7PMN61Q:~/test1$ rm 12345
seirena1377@DESKTOP-7PMN61Q:~/test1$ ls -la
total 40
drwxr-xr-x 3 seirena1377 seirena1377 4096 Sep 26 23:20  .
drwxr-xr-x 6 seirena1377 seirena1377 4096 Sep 22 01:18  ..
drwxr-xr-x 8 seirena1377 seirena1377 4096 Sep 26 23:20  .git
-rw-r--r-- 1 seirena1377 seirena1377   64 Sep 22 22:21  789.txt
-rw-r--r-- 1 seirena1377 seirena1377  742 Sep 22 22:22  INFO.md
-rw-r--r-- 1 seirena1377 seirena1377   87 Sep 16 23:49  README.md
-rw-r--r-- 1 seirena1377 seirena1377 1395 Sep 22 22:11  file-feature-2.txt
-rw-r--r-- 1 seirena1377 seirena1377 2468 Sep 26 23:02  file-main-feature.txt
-rw-r--r-- 1 seirena1377 seirena1377 6106 Sep 16 23:49 'Дом питомца.xlsx'
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git add .
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ commit -am "удален файл 12345"
commit: command not found
seirena1377@DESKTOP-7PMN61Q:~/test1$ git commit -am "удален файл 12345"
[master 3a453d0] удален файл 12345
 1 file changed, 1 deletion(-)
 delete mode 100644 12345
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Already up to date.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin master
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 239 bytes | 239.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Seirena/test1.git
   34c6ae2..3a453d0  master -> master
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout 15-4-feature-1
Switched to branch '15-4-feature-1'
seirena1377@DESKTOP-7PMN61Q:~/test1$ nano NEW.jason
seirena1377@DESKTOP-7PMN61Q:~/test1$ git add .
seirena1377@DESKTOP-7PMN61Q:~/test1$ git commit -am "новый джэйсон файл"
[15-4-feature-1 3957f3c] новый джэйсон файл
 1 file changed, 2 insertions(+)
 create mode 100644 NEW.jason
seirena1377@DESKTOP-7PMN61Q:~/test1$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
seirena1377@DESKTOP-7PMN61Q:~/test1$ git merge 15-4-feature-1
Merge made by the 'recursive' strategy.
 NEW.jason | 2 ++
 1 file changed, 2 insertions(+)
 create mode 100644 NEW.jason
seirena1377@DESKTOP-7PMN61Q:~/test1$ git push origin master
Username for 'https://github.com': seirena
Password for 'https://seirena@github.com':
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 536 bytes | 536.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Seirena/test1.git
   3a453d0..c5c9737  master -> master
