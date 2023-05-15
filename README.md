Terminal history




walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "First file in git" > file1.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "making an html file" > file2.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ echo "making a css file" > file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ ls
README.md  file1.txt  file2.html  file3.css

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
   0adaad0..b27b74c  main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git branch -b dev
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch
* dev
  main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch test

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch
* dev
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
README.md  file1.txt  file2.html  file3.css

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
remote:      https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ git branch -d test
Deleted branch test (was b27b74c).

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$ ^C

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (dev)
$



Bundle 2





walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git branch ft/services-redesign

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/services-redesign
Switched to branch 'ft/services-redesign'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ ls
README.md  file1.txt  file2.html  file3.css

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ touch service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git commit -a -m "updating service.html"
On branch ft/services-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git commit -m "updating service.html"
[ft/services-redesign e2e6011] updating service.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git push
fatal: The current branch ft/services-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/services-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git push origin ft/services-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 284 bytes | 284.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/services-redesign' on GitHub by visiting:
remote:      https://github.com/AristideI/Gym-Git-Exercise-Solutions/pull/new/ft/services-redesign
remote:
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/services-redesign -> ft/services-redesign

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git merge ft/services-redesign
Updating cf6d11b..e2e6011
Fast-forward
 service.html | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "updating service to branch main"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
sTotal 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   cf6d11b..e2e6011  main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "updating service to branch main"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ ls
README.md  file1.txt  file2.html  file3.css  service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ vi service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add .
warning: in the working copy of 'service.html', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git commit -m "updating service"
[main cae44aa] updating service
 1 file changed, 1 insertion(+)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 268 bytes | 268.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   e2e6011..cae44aa  main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git branch ft/services-redesign
fatal: a branch named 'ft/services-redesign' already exists

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/services-redesign
Switched to branch 'ft/services-redesign'

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ vi service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ vi service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git add .
warning: in the working copy of 'service.html', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git commit -m "saint"
[ft/services-redesign de7512d] saint
 1 file changed, 1 insertion(+)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git push origin ft/services-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 254 bytes | 254.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   e2e6011..de7512d  ft/services-redesign -> ft/services-redesign

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/services-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git merge ft/services-redesign
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main|MERGING)
$ vi service.html

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main|MERGING)
$ git add .

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main|MERGING)
$ git commit -m "mergin ft/service-redesign"
[main 23d28d4] mergin ft/service-redesign

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 226 bytes | 226.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
   cae44aa..23d28d4  main -> main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"

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





Bundle 3










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

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$

