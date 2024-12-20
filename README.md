# Gym-Git-Exercises-Solution
## Bundle 1
### Exercise 1

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
$

#### Bundle 1
##### Exercises 2

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
##### Bundle 2
###### Exercise 1
