
walte@Walter MINGW64 ~
$ cd d:

walte@Walter MINGW64 /d
$ ls
'$RECYCLE.BIN'/   Alx/  'System Volume Information'/  'The Gym'/

walte@Walter MINGW64 /d
$ cd The\ Gym/

walte@Walter MINGW64 /d/The Gym
$ ls
Gym-Git-Exercise-Solutions/  PLD/  youtube/

walte@Walter MINGW64 /d/The Gym
$ cs Gym-Git-Exercise-Solutions/
bash: cs: command not found

walte@Walter MINGW64 /d/The Gym
$ cd Gym-Git-Exercise-Solutions/

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions
$ echo "the saint" > pro.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions
$ git add .
fatal: not a git repository (or any of the parent directories): .git

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions
$ git inti
git: 'inti' is not a git command. See 'git --help'.

The most similar command is
        init

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions
$ git init
Initialized empty Git repository in D:/The Gym/Gym-Git-Exercise-Solutions/.git/

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master)
$ git add .
warning: in the working copy of 'pro.txt', LF will be replaced by CRLF the next time Git touches it

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master)
$ git commit -m "The saint"
[master (root-commit) 91d5178] The saint
 1 file changed, 1 insertion(+)
 create mode 100644 pro.txt

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (master)
$ git branch -m master main

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git remote add origin https://github.com/AristideI/Gym-Git-Exercise-Solutions.git

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push -u main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push origin main
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/AristideI/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 655 bytes | 19.00 KiB/s, done.
From https://github.com/AristideI/Gym-Git-Exercise-Solutions
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push origin main
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/AristideI/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git pull https://github.com/AristideI/Gym-Git-Exercise-Solutions.git main
From https://github.com/AristideI/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$ git push -f origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 225 bytes | 225.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AristideI/Gym-Git-Exercise-Solutions.git
 + 6c641a6...91d5178 main -> main (forced update)

walte@Walter MINGW64 /d/The Gym/Gym-Git-Exercise-Solutions (main)
$

