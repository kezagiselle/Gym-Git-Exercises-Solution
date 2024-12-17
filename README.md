# Gym-Git-Exercises-Solution
lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ git branch master

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ git checkout -b master
fatal: a branch named 'master' already exists

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (main)
$ git checkout master
Switched to branch 'master'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git add .

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git commit -m "made some changes"
[master ba9d530] made some changes
 1 file changed, 18 insertions(+)
 create mode 100644 index.html

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git clone https://github.com/kezagiselle/DOMExercises.git
Cloning into 'DOMExercises'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 9 (delta 1), reused 5 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (9/9), done.
Resolving deltas: 100% (1/1), done.

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git add .
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
$ git add DOMExercises

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git commit -m "Added another repo in my project"
[master 6d4bbc7] Added another repo in my project
 1 file changed, 1 insertion(+)
 create mode 160000 DOMExercises

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git branch dev

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (master)
$ git checkout dev
Switched to branch 'dev'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)
$ git branch test

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)
$ git checkout test
Switched to branch 'test'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (test)
$ git checkout dev
Switched to branch 'dev'

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)
$ git branch -d test
Deleted branch test (was 6d4bbc7).

lenovo@DESKTOP-QR2DGVN MINGW64 ~/Desktop/Gym-Git-Exercises-Solution (dev)
$