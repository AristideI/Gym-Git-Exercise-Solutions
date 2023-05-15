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

