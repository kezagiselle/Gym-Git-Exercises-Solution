# Gym-Git-Exercises-Solution
## Bundle 1
### Exercise 1
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

#### Bundle 1
##### Exercises 2
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
##### Bundle 2
###### Exercise 1
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

### Exercise 2
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

#### Bundle 3
### Exercise 1
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

