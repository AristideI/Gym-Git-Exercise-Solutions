Terminal history

"""
bash

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions $ git init Initialized empty Git repository in D:/The Gym/Gym-Git-Exercise-Solutions/.git/
=======
>>>>>>> 1b21e9166eea58407727b967dad94280ee41ff0d


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'file2.html', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'file3.css', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "initial commit to my github repo"
[main b27b74c] initial commit to my github repo


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (5/5), 431 bytes | 431.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch test

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "making new branch dev"
On branch dev
nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ls

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ vi file1.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git add .
warning: in the working copy of 'file1.txt', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git commit -m "making new branch dev"


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
h]      dev -> dev


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was b27b74c).

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ^C

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$

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
bash

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "pushing merged files"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ ^C

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$
E





#Bundle 3










walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ ls
README.md  file1.txt  file2.html  file3.css  service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ vi team.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m "making changes in team.html"
[ft/team-page b9a15ad] making changes in team.html
 1 file changed, 3 insertions(+)
 create mode 100644 team.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 307 bytes | 307.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log
OBcommit b9a15ad4be4e7c212897db283c96b6eeb744b223 (HEAD -> ft/team-page, origin/ft/team-page)
Author: aristidei <a.isingizwe@alustudent.com>
OBDate:   Mon May 15 14:07:54 2023 +0200

OB    making changes in team.html

OBcommit 461b1e3b658b8bc634342089b346d37deca21d79 (origin/main, main, ft/contact-page)
OBAuthor: aristidei <a.isingizwe@alustudent.com>
OBDate:   Mon May 15 02:45:12 2023 +0200
OB
    updating terminal history

commit 23d28d404ef821ef213cf72f3508dcb1dbdd6a99
Merge: cae44aa de7512d
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:42:38 2023 +0200

    mergin ft/service-redesign

commit de7512d7b53c11d0189e55f784d3771cce450494 (origin/ft/services-redesign, ft/services-redesign)
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:39:54 2023 +0200

    saint

commit cae44aa9cb654c24f1c7473b0fff8d9808f9a26e
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:37:42 2023 +0200

    updating service

commit e2e6011bd877adac28e5e709666c85ea075aaa5b
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:24:32 2023 +0200

    updating service.html

commit cf6d11b15fd37d6cf90bc2ee1d0166b3a87da45b
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Sun May 14 15:25:18 2023 +0200

    updating terminal history

commit b27b74c6e466314a639f0974feac16f60c3a789e
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Sun May 14 15:12:52 2023 +0200


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git cherry-pick b9a15ad4be4e7c212897db283c96b6eeb744b223
[ft/contact-page 9cb7828] making changes in team.html
 Date: Mon May 15 14:07:54 2023 +0200
 1 file changed, 3 insertions(+)
 create mode 100644 team.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push --all
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/contact-page)





walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ touch faq.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m "creating faq page"
[ft/faq-page f128890] creating faq page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 faq.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 272 bytes | 272.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git log
commit f1288905bdcca9d2a5afb60dde684957e025e912 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 15:37:17 2023 +0200

    creating faq page

commit b3016afea7f15364ae0e3fbc172eed4384c84e2c (origin/ft/contact-page, ft/contact-page)
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 14:40:35 2023 +0200

    updating terminal history

commit 9cb7828ed1ed3cdf4b5bec261f03fd7da5e86c5c
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 14:07:54 2023 +0200

    making changes in team.html

commit 461b1e3b658b8bc634342089b346d37deca21d79 (origin/main, main)
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:45:12 2023 +0200

    updating terminal history

commit 23d28d404ef821ef213cf72f3508dcb1dbdd6a99
Merge: cae44aa de7512d
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:42:38 2023 +0200

    mergin ft/service-redesign

commit de7512d7b53c11d0189e55f784d3771cce450494 (origin/ft/services-redesign, ft/services-redesign)
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:39:54 2023 +0200

    saint

commit cae44aa9cb654c24f1c7473b0fff8d9808f9a26e
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:37:42 2023 +0200

    updating service

commit e2e6011bd877adac28e5e709666c85ea075aaa5b
Author: aristidei <a.isingizwe@alustudent.com>
Date:   Mon May 15 02:24:32 2023 +0200


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git revert f1288905bdcca9d2a5afb60dde684957e025e912
[ft/faq-page 052ea00] Revert "creating faq page"
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 faq.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m "reverting to last commit "
On branch ft/faq-page
nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 259 bytes | 259.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   f128890..052ea00  ft/faq-page -> ft/faq-page

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git branch main
fatal: a branch named 'main' already exists

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ touch new

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "making changes in main"
[main 3270439] making changes in main
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 273 bytes | 273.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   461b1e3..3270439  main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ ls
README.md  file1.txt  file2.html  file3.css  new  service.html  team.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ vi file1.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m "rebasing the main"
[ft/home-page-redesign e67e09b] rebasing the main
 1 file changed, 1 insertion(+)

"""
