# Gym-Git-Exercises-Solution
## Bundle 1
## Exercise 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git branch master`
$ `git branch master`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout -b master`

fatal: a branch named 'master' already exists

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout master`

Switched to branch 'master'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git add.`

git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git commit -m "made some changes"`

[master ba9d530] made some changes
 1 file changed, 18 insertions(+)
 create mode 100644 index.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git clone https://github.com/kezagiselle/DOMExercises.git`

Cloning into 'DOMExercises'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 9 (delta 1), reused 5 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (9/9), done.
Resolving deltas: 100% (1/1), done.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git add .`

warning: adding embedded git repository: DOMExercises
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it. 
hint: If you meant to add a submodule, use:
hint: 
hint:   git submodule add <url> DOMExercises
hint: 
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint: 
hint:   git rm --cached DOMExercises
hint: 
hint: See "git help submodule" for more information.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ ^C

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git add DOMExercises`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git commit -m "Added another repo in my project"`

[master 6d4bbc7] Added another repo in my project
 1 file changed, 1 insertion(+)
 create mode 160000 DOMExercises

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ `git branch dev`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)

$ `git checkout dev`
Switched to branch 'dev'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)

$ `git branch test`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)

$ `git checkout test`
Switched to branch 'test'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (test)

$ `git checkout dev`
Switched to branch 'dev'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)

$ `git branch -d test`
Deleted branch test (was 6d4bbc7).

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)
```


## Exercises 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash`
Saved working directory and index state WIP on main: 3cb824a added my solutions on the Readme file

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash`
Saved working directory and index state WIP on main: 3cb824a added my solutions on the Readme file

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash pop about.html`
error: about.html is not a valid reference

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git add about.html`
fatal: pathspec 'about.html' did not match any files

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash pop`
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (a0e37f6ac10c185df7f30d4c00d1b2a768e64c93) 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash pop`
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

Dropped refs/stash@{0} (15c004ddb331bf05cf47c9693de70acdb0a59c86)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git add about.html`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash push -m "stash changes for about.html" --about.html`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash`
Saved working directory and index state WIP on main: 3cb824a added my solutions on the Readme file

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash list`
stash@{0}: WIP on main: 3cb824a added my solutions on the Readme file

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash pop stash@{1}`
fatal: log for 'stash' only has 1 entries

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git stash pop stash@{0}`
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (8a3aca4f512e65646c8794cba09ecebef5ec3e9f)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git commit -m "current changes"`
[main 093724c] current changes
 3 files changed, 54 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git status`
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git reset`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git checkout -- team.html`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git status`
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git push`
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 361 bytes | 361.00 KiB/s, done.      
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
   70e804c..093724c  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ `git status`
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Bundle 2
## Exercise 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git branch ft/bundle-2`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add service.html`
fatal: pathspec 'service.html' did not match any files

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "created a new file which is service.html"`

[main 2a3fbdd] created a new file which is service.html
 2 files changed, 20 insertions(+)
 create mode 100644 services.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 345 bytes | 115.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
   3fef5a2..2a3fbdd  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git pull`

Already up to date.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git branch ft/service-redesign`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "made some changes on service.html"`
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`
```

## Exercise 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout -b ft/service.redesign`
Switched to a new branch 'ft/service.redesign'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git push`

fatal: The current branch ft/service.redesign has no upstream branch.
To push the current branch and set the remote as upstream, use    

    git push --set-upstream origin ft/service.redesign

To have this happen automatically for branches without a tracking 
upstream, see 'push.autoSetupRemote' in 'git help config'.        


lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git push origin`

fatal: The current branch ft/service.redesign has no upstream branch.
To push the current branch and set the remote as upstream, use    

    git push --set-upstream origin ft/service.redesign

To have this happen automatically for branches without a tracking 
upstream, see 'push.autoSetupRemote' in 'git help config'.        


lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git push ft/service-redesign`

fatal: 'ft/service-redesign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git push origin ft/service-redesign`

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub 
by visiting:
remote:      https://github.com/kezagiselle/Gym-Git-Exercises-Solution/pull/new/ft/service-redesign
remote:
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
 * [new branch]      ft/service-redesign -> ft/service-redesign   

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git checkout -b main`

fatal: a branch named 'main' already exists

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service.redesign)

$ `git checkout main`

Switched to branch 'main'
M       services.html
Your branch is up to date with 'origin/main'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "changes"`
[main 89b84e2] changes
 1 file changed, 2 insertions(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin mai`

error: src refspec mai does not match any
error: failed to push some refs to 'https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 288 bytes | 288.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
   2a3fbdd..89b84e2  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git diff`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/service-redesign`

error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
Everything up-to-date

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/services-redesign`

error: pathspec 'ft/services-redesign' did not match any file(s) known to git

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/service-redesign`

error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout-b ft/service-redesign`

git: 'checkout-b' is not a git command. See 'git --help'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout -b ft/service-redesign`
fatal: a branch named 'ft/service-redesign' already exists

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/service-redesign`

error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "changes on services.html"`

[main 2aefba2] changes on services.html
 1 file changed, 1 insertion(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 300 bytes | 300.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
   89b84e2..2aefba2  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/service-redesign`

Switched to branch 'ft/service-redesign'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git commit -m "changes on my new branch"`

On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git commit -m "changes on my new branch"`

On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git commit -m "changes on my new branch"`
[ft/service-redesign 474e198] changes on my new branch
 1 file changed, 1 insertion(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git push`

fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use    

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking 
upstream, see 'push.autoSetupRemote' in 'git help config'.        


lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git push origin ft/service-redesign`

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 295 bytes | 295.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
   2a3fbdd..474e198  ft/service-redesign -> ft/service-redesign   

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)

$ `git diff`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/service-redesign)
$
```

## Bundle 3
## Exercise 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/contact-page)

$ `git checkout ft/team-page`
Switched to branch 'ft/team-page'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/team-page)

$ `git checkout ft/contact-page`
Switched to branch 'ft/contact-page'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/contact-page)

$ `git checkout ft/faq-page`
error: pathspec 'ft/faq-page' did not match any file(s) known to git

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/contact-page)

$ `git checkout ft/faq-page`
error: pathspec 'ft/faq-page' did not match any file(s) known to git

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/contact-page)

$ `git branch ft/faq-page`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/contact-page)

$ `git checkout ft/faq-page`
Switched to branch 'ft/faq-page'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/faq-page)
$
the rest of codes were about PR on Github
```

## Exercise 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/faq-page)

$ `git checkout ft/home-page-redesign`
Switched to branch 'ft/home-page-redesign'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign)

$ `git checkout main`
Switched to branch 'main'

Your branch is behind 'origin/main' by 13 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "changes on the main"`
[main 172e00e] changes on the main
 1 file changed, 2 insertions(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/home-page-redesign`
Switched to branch 'ft/home-page-redesign'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign)

$ `git rebase`
There is no tracking information for the current branch.
Please specify which branch you want to rebase against.
See git-rebase(1) for details.

    git rebase '<branch>'

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=<remote>/<branch> ft/home-page-redesign

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign)

$ `git rebase main`
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
error: could not apply cd7be99... made some changes in the team.html
hint: Resolve all conflicts manually, mark them as resolved with  
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".  
hint: To abort and get back to the state before "git rebase", run 
"git rebase --abort".
Could not apply cd7be99... made some changes in the team.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)
$ ^C

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$  `git add/rm team.html`
git: 'add/rm' is not a git command. See 'git --help'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git add team.html`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git rebase main`
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something 
valuable there.


lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git commit -m "did some changes"`
[detached HEAD bad8544] did some changes
 2 files changed, 5 insertions(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git push origin ft/home-page-redesign`
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/kezagiselle/Gym-Git-Exercises-Solution/pull/new/ft/home-page-redesign
remote:
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 6/9)

$ `git checkout main`
error: Your local changes to the following files would be overwritten by checkout:
        README.md
Please commit your changes or stash them before you switch branches.
Aborting

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git commit -m "changes on this branch"`
[detached HEAD 5adabd7] changes on this branch
 1 file changed, 9 insertions(+), 6 deletions(-)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git push origin ft/home-page-redesign`
Everything up-to-date

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git checkout main`
Warning: you are leaving 8 commits behind, not connected to
any of your branches:

  5adabd7 changes on this branch
  3a0766b made some changes in the team.html
  bad8544 did some changes
  1454843 did some changes
 ... and 4 more.

If you want to keep them by creating a new branch, this may be a good time
to do so with:

 git branch <new-branch-name> 5adabd7

Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 13 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git pull origin main`
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 2.59 KiB | 189.00 KiB/s, done.
From https://github.com/kezagiselle/Gym-Git-Exercises-Solution
 * branch            main       -> FETCH_HEAD
   8edb7fa..826683f  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 390 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 faq.html  |  23 ++++
 team.html |   4 +
 3 files changed, 414 insertions(+), 3 deletions(-)
 create mode 100644 faq.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign|REBASE 7/9)

$ `git rebase --abort`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/home-page-redesign)

$ `git checkout main`
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Bundle 4
## Exercise 1
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git remote add git-copy https://github.com/kezagiselle/git-copy.git`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "made changes on the on home file"`
[main d472698] made changes on the on home file
 1 file changed, 1 insertion(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 306 bytes | 306.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
   efc67e9..d472698  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push git-copy`
To https://github.com/kezagiselle/git-copy.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kezagiselle/git-copy.git'
hint: Updates were rejected because the remote contains work that 
you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote 
changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for 
details.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "some changes"`
[main 2b89848] some changes
 1 file changed, 1 insertion(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push git-copy`
To https://github.com/kezagiselle/git-copy.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kezagiselle/git-copy.git'
hint: Updates were rejected because the remote contains work that 
you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote 
changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for 
details.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Exercise 2
```bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/footer`
Switched to branch 'ft/footer'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git commit -m "first commit on this branch"`
[ft/footer 481a658] first commit on this branch
 1 file changed, 1 insertion(+)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git push origin ft/footer`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 292 bytes | 292.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/kezagiselle/Gym-Git-Exercises-Solution/pull/new/ft/footer
remote:
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
 * [new branch]      ft/footer -> ft/footer

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git commit -m "second commit on this branch"`
[ft/footer 3d3829f] second commit on this branch
 1 file changed, 2 insertions(+), 1 deletion(-)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git push origin ft/footer`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
   481a658..3d3829f  ft/footer -> ft/footer

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/footer)

$ `git checkout main`
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git branch ft/squashing`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git merge --squash ft/footer`
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
Squash commit -- not updating HEAD
Automatic merge failed; fix conflicts and then commit the result. 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git merge --squash ft/footer`
error: Your local changes to the following files would be overwritten by merge:
  team.html
<stdin>:10: trailing whitespace.

warning: 1 line adds whitespace errors.
Merge with strategy ort failed.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "changes"`
[main df812ff] changes
 1 file changed, 2 insertions(+), 1 deletion(-)

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git'
hint: Updates were rejected because the remote contains work that 
you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote 
changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for 
details.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git merge --squash ft/footer`
Automatic merge went well; stopped before committing as requested
Squash commit -- not updating HEAD

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "squashed changes"`
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git'
hint: Updates were rejected because the remote contains work that 
you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote 
changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for 
details.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m "footer changes squashing"`
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push`
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git'
hint: Updates were rejected because the remote contains work that 
you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote 
changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for 
details.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Bundle 5
## Exercise 1
it's done on Github 

## Exercise 2
``` bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git clone https://github.com/TheGymRwanda/git-cafe-exercise.git`
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 92 (fReceiving objects: 100% (107/107), 1.95 MiB | 1.86 MiB/s, done.   

Resolving deltas: 100% (5/5), done.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git commit -m " changes on the index file"`
[main 4cea631]  changes on the index file
 2 files changed, 4 insertions(+)
 create mode 160000 git-cafe-exercise

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git push origin main`
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 383 bytes | 383.00 KiB/s, done.      
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git
   5afed0d..4cea631  main -> main

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Bundle 6
## Exercise 1
``` bash
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git branch ft/cafe`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout ft/cafe`
Switched to branch 'ft/cafe'
M       git-cafe-exercise

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git commit -m "changes on this branch"`
On branch ft/cafe
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git commit -m "changes on this branch"`
On branch ft/cafe
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git add git-cafe-exercise`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)

$ `git commit -m "changes on this branch"`
On branch ft/cafe
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (ft/cafe)
$
```
## Exercise 2
``` bash

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)

$ `git checkout -b bugfix`
Switched to a new branch 'bugfix'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git commit -m "changed the index-4 file"`
On branch bugfix
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git status`
On branch bugfix
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git add git-cafe-exercise`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git  commit -m "describe the changes"`
On branch bugfix
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)      
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)
        modified:   git-cafe-exercise (modified content)

no changes added to commit (use "git add" and/or "git commit -a") 

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git add .`

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git push origin ft/bugfix`
error: src refspec ft/bugfix does not match any
error: failed to push some refs to 'https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git push origin bugfix`
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'bugfix' on GitHub by visiting: 
remote:      https://github.com/kezagiselle/Gym-Git-Exercises-Solution/pull/new/bugfix
remote:
To https://github.com/kezagiselle/Gym-Git-Exercises-Solution.git  
 * [new branch]      bugfix -> bugfix

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (bugfix)

$ `git checkout main`
Switched to branch 'main'
M       git-cafe-exercise
Your branch is up to date with 'origin/main'.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$
```
## Exercise 3




