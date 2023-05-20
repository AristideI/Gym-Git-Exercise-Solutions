Terminal history

"""
bash

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions $ git init Initialized empty Git repository in D:/The Gym/Gym-Git-Exercise-Solutions/.git/

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master) $ git add . warning: in the working copy of 'pro.txt', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master) $ git commit -m "The saint" [master (root-commit) 91d5178] The saint 1 file changed, 1 insertion(+) create mode 100644 pro.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master) $ git branch -m master main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git remote add origin https://github.com/AristideI/Gym-Git-Exercise-Solutions.git

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git push -u main fatal: 'main' does not appear to be a git repository fatal: Could not read from remote repository.

Please make sure you have the correct access rights and the repository exists.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git push fatal: The current branch main has no upstream branch. To push the current branch and set the remote as upstream, use

git push --set-upstream origin main
To have this happen automatically for branches without a tracking upstream, see 'push.autoSetupRemote' in 'git help config'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git pull remote: Enumerating objects: 3, done. remote: Counting objects: 100% (3/3), done. remote: Compressing objects: 100% (2/2), done. remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 Unpacking objects: 100% (3/3), 655 bytes | 19.00 KiB/s, done. From https://github.com/AristideI/Gym-Git-Exercise-Solutions

[new branch] main -> origin/main There is no tracking information for the current branch. Please specify which branch you want to merge with. See git-pull(1) for details.

git pull

If you wish to set tracking information for this branch you can do so with:

git branch --set-upstream-to=origin/<branch> main
walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git push origin main To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git ! [rejected] main -> main (non-fast-forward) error: failed to push some refs to 'https://github.com/AristideI/Gym-Git-Exercise-Solutions.git' hint: Updates were rejected because the tip of your current branch is behind hint: its remote counterpart. Integrate the remote changes (e.g. hint: 'git pull ...') before pushing again. hint: See the 'Note about fast-forwards' in 'git push --help' for details.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git pull https://github.com/AristideI/Gym-Git-Exercise-Solutions.git main From https://github.com/AristideI/Gym-Git-Exercise-Solutions

branch main -> FETCH_HEAD fatal: refusing to merge unrelated histories
walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $ git push -f origin main Enumerating objects: 3, done. Counting objects: 100% (3/3), done. Writing objects: 100% (3/3), 225 bytes | 225.00 KiB/s, done. Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git

6c641a6...91d5178 main -> main (forced update)
walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main) $

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "First file in git" > file1.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "making an html file" > file2.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "making a css file" > file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ ls
README.md file1.txt file2.html file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'file2.html', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'file3.css', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "initial commit to my github repo"
[main b27b74c] initial commit to my github repo
3 files changed, 3 insertions(+)
create mode 100644 file1.txt
create mode 100644 file2.html
create mode 100644 file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (5/5), 431 bytes | 431.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
0adaad0..b27b74c main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch

- dev
  main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch test

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch

- dev
  main
  test

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "making new branch dev"
On branch dev
nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ls
README.md file1.txt file2.html file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi file1.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "making new branch dev"
[dev 35d526a] making new branch dev
1 file changed, 1 insertion(+), 1 deletion(-)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 284 bytes | 284.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote: https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git

- [new branch] dev -> dev

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was b27b74c).

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ^C

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ ls
README.md file1.txt file2.html file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout dev
Switched to branch 'dev'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ls
README.md file1.txt file2.html file3.css home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ rm home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ touch home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "Exercise 2"
[dev 1e501bd] Exercise 2
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state WIP on dev: 1e501bd Exercise 2

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash push -m "about"
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state On dev: about

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi home.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash push -m "team"
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state On dev: team

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash pop about
error: about is not a valid reference

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash pop "about"
error: about is not a valid reference

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: On dev: team
stash@{1}: On dev: about
stash@{2}: WIP on dev: 1e501bd Exercise 2

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash pop 1
On branch dev
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: home.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{1} (53256a036c9e687f935f44422ce99c4b9a2cf21d)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash pop 1
error: Your local changes to the following files would be overwritten by merge:
home.html
Please commit your changes or stash them before you merge.
Aborting
On branch dev
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: home.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "editing new pages to dev branch"
[dev 2f5aed0] editing new pages to dev branch
1 file changed, 1 insertion(+)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 519 bytes | 519.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
d6c417b..2f5aed0 dev -> dev

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: On dev: team
stash@{1}: WIP on dev: 1e501bd Exercise 2

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git stash pop 1
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html
On branch dev
Unmerged paths:
(use "git restore --staged <file>..." to unstage)
(use "git add <file>..." to mark resolution)
both modified: home.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git log
commit 2f5aed0f7ff2c2243a0e767d28bb937358d0635b (HEAD -> dev, origin/dev)
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:51:42 2023 +0200

    editing new pages to dev branch

commit 1e501bd69b2cb993b88ea23319efae8d3b058bdd
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:40:05 2023 +0200

    Exercise 2

commit d6c417b03361fbfd664826cdbf14736cfeb2c293
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:23:01 2023 +0200

    upsate terminal history

commit 35d526a0f0c3b98424b017bae0ae1e60165ba1ca
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:19:59 2023 +0200

    making new branch dev

commit b27b74c6e466314a639f0974feac16f60c3a789e
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:12:52 2023 +0200

    initial commit to my github repo

commit 0adaad0881bd3b0c63b78338b4ee111c7d7426e7
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:07:49 2023 +0200

    creating terminal history readme

commit 497436f60f83ffe7171bdcdf22fdae186d0e7968
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:05:41 2023 +0200

    the saint

commit 67e8ec584164e36f016401bba7e6c06d5fc5a98c
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 14:59:20 2023 +0200

    removing sample files

commit 882cc0fa215c9108fd4fbc2c37d222f75035ea06
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 12:37:17 2023 +0200

    adding readme containing terminal history

commit 91d517858c7cc04dc66019a413526c7d01232fc3
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 12:27:27 2023 +0200

    The saint

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git log
commit 2f5aed0f7ff2c2243a0e767d28bb937358d0635b (HEAD -> dev, origin/dev)
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:51:42 2023 +0200

    editing new pages to dev branch

commit 1e501bd69b2cb993b88ea23319efae8d3b058bdd
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:40:05 2023 +0200

    Exercise 2

commit d6c417b03361fbfd664826cdbf14736cfeb2c293
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:23:01 2023 +0200

    upsate terminal history

commit 35d526a0f0c3b98424b017bae0ae1e60165ba1ca
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:19:59 2023 +0200

    making new branch dev

commit b27b74c6e466314a639f0974feac16f60c3a789e
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:12:52 2023 +0200

    initial commit to my github repo

commit 0adaad0881bd3b0c63b78338b4ee111c7d7426e7
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:07:49 2023 +0200

    creating terminal history readme

commit 497436f60f83ffe7171bdcdf22fdae186d0e7968
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:05:41 2023 +0200

    the saint

commit 67e8ec584164e36f016401bba7e6c06d5fc5a98c
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 14:59:20 2023 +0200

    removing sample files

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git log -p
commit 2f5aed0f7ff2c2243a0e767d28bb937358d0635b (HEAD -> dev, origin/dev)
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:51:42 2023 +0200

    editing new pages to dev branch

diff --git a/home.html b/home.html
index e69de29..6b914f0 100644
--- a/home.html
+++ b/home.html
@@ -0,0 +1 @@
+Added stash called about

commit 1e501bd69b2cb993b88ea23319efae8d3b058bdd
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 16:40:05 2023 +0200

   # Exercise 2

diff --git a/home.html b/home.html
new file mode 100644
index 0000000..e69de29

commit d6c417b03361fbfd664826cdbf14736cfeb2c293
Author: aristidei <a.isingizwe@alustudent.com>
Date: Sun May 14 15:23:01 2023 +0200

    upsate terminal history

diff --git a/README.md b/README.md
index da95aeb..9f87dd6 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,161 @@
Terminal history

-
-
-
- +walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
  +$ echo "First file in git" > file1.txt
- +walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
  +$ echo "making an html file" > file2.html
- +walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
  +$ echo "making a css file" > file3.css
-

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git reset --hard 2f5aed0f7ff2c2243a0e767d28bb937358d0635b
HEAD is now at 2f5aed0 editing new pages to dev branch

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git push origin dev
Everything up-to-date

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi README.md

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)


"""
