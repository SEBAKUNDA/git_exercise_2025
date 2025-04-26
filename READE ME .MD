#Git exercise project

This project will be used for series of git exercise

#bash1#
```bash
 The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git status
On branch main
nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
* main
192:exercises_2025 eric$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   READE ME .MD

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"innitial commit"
[main 4a004ae] innitial commit
 1 file changed, 1 insertion(+), 1 deletion(-)
192:exercises_2025 eric$ git remote add 
 *  History restored 


The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git status
On branch main
nothing to commit, working tree clean
192:exercises_2025 eric$ git remote add origin https://github.com/SEBAKUNDA/git_exercise_2025.git
192:exercises_2025 eric$ git status
On branch main
nothing to commit, working tree clean
192:exercises_2025 eric$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

192:exercises_2025 eric$    git push --set-upstream origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (9/9), 751 bytes | 375.00 KiB/s, done.
Total 9 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
192:exercises_2025 eric$ git checkout dev
error: pathspec 'dev' did not match any file(s) known to git
192:exercises_2025 eric$ git checkout -b
error: switch `b' requires a value
192:exercises_2025 eric$ git checkout - b dev
error: pathspec '-' did not match any file(s) known to git
error: pathspec 'b' did not match any file(s) known to git
error: pathspec 'dev' did not match any file(s) known to git
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git push
Everything up-to-date
192:exercises_2025 eric$ git checkout dev
error: pathspec 'dev' did not match any file(s) known to git
192:exercises_2025 eric$ git checkout -b dev
Switched to a new branch 'dev'
192:exercises_2025 eric$ git status
On branch dev
nothing to commit, working tree clean
192:exercises_2025 eric$ git push origin dev
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/git_exercise_2025/pull/new/dev
remote: 
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 * [new branch]      dev -> dev
192:exercises_2025 eric$ git checkout -d test
error: unknown switch `d'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -q, --quiet           suppress progress reporting
    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --detach              detach HEAD at named commit
    -t, --track           set upstream info for new branch
    --orphan <new-branch>
                          new unparented branch
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -f, --force           force checkout (throw away local modifications)
    -m, --merge           perform a 3-way merge with the new branch
    --overwrite-ignore    update ignored files (default)
    --conflict <style>    conflict style (merge or diff3)
    -p, --patch           select hunks interactively
    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --ignore-other-worktrees
                          do not check if another worktree is holding the given ref
    --recurse-submodules[=<checkout>]
                          control recursive updating of submodules
    --progress            force progress reporting

192:exercises_2025 eric$ git checkout -b test
Switched to a new branch 'test'
192:exercises_2025 eric$ git push origim test
fatal: 'origim' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
192:exercises_2025 eric$ git push origin test
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/git_exercise_2025/pull/new/test
remote: 
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 * [new branch]      test -> test
192:exercises_2025 eric$ git checkout dev
Switched to branch 'dev'
192:exercises_2025 eric$ git branch 
* dev
  main
  test
192:exercises_2025 eric$ git checkout test
Switched to branch 'test'
192:exercises_2025 eric$ git branch 
  dev
  main
* test
192:exercises_2025 eric$ git checkout dev
Switched to branch 'dev'
192:exercises_2025 eric$ git branch
* dev
  main
  test
192:exercises_2025 eric$ git branch -D test
Deleted branch test (was 4a004ae).
192:exercises_2025 eric$ git branch
* dev
  main
192:exercises_2025 eric$ git push origin --delete test
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 - [deleted]         test
192:exercises_2025 eric$ git branch 
* dev
  main
192:exercises_2025 eric$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   home.html

192:exercises_2025 eric$ git stash list
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   home.html

192:exercises_2025 eric$ git stash 
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash list 
stash@{0}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git status
On branch dev
nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        About.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html

192:exercises_2025 eric$ git stash 
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash list 
stash@{0}: WIP on dev: 4a004ae innitial commit
stash@{1}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        team.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

192:exercises_2025 eric$ git stash
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash list
stash@{0}: WIP on dev: 4a004ae innitial commit
stash@{1}: WIP on dev: 4a004ae innitial commit
stash@{2}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash pop
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

Dropped refs/stash@{0} (4ac35322e5f1c81e8121f9f903bd564548521a60)
192:exercises_2025 eric$ git sta list 
git: 'sta' is not a git command. See 'git --help'.

The most similar commands are
        status
        stage
        stash
192:exercises_2025 eric$ git stash list 
stash@{0}: WIP on dev: 4a004ae innitial commit
stash@{1}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash team.html
usage: git stash list [<options>]
   or: git stash show [<stash>]
   or: git stash drop [-q|--quiet] [<stash>]
   or: git stash ( pop | apply ) [--index] [-q|--quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash save [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                      [-u|--include-untracked] [-a|--all] [<message>]
   or: git stash [push [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                       [-u|--include-untracked] [-a|--all] [-m <message>]
                       [-- <pathspec>...]]
   or: git stash clear
192:exercises_2025 eric$ git stash add team.html
usage: git stash list [<options>]
   or: git stash show [<stash>]
   or: git stash drop [-q|--quiet] [<stash>]
   or: git stash ( pop | apply ) [--index] [-q|--quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash save [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                      [-u|--include-untracked] [-a|--all] [<message>]
   or: git stash [push [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                       [-u|--include-untracked] [-a|--all] [-m <message>]
                       [-- <pathspec>...]]
   or: git stash clear
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

192:exercises_2025 eric$ git stash 
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash 
No local changes to save
192:exercises_2025 eric$ git stash list 
stash@{0}: WIP on dev: 4a004ae innitial commit
stash@{1}: WIP on dev: 4a004ae innitial commit
stash@{2}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

Dropped stash@{0} (b5eff47e8be98798e51384f84d8650cb52c052c5)
192:exercises_2025 eric$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   team.html

Dropped stash@{0} (b2aba75fec812419a64f04f5088e7565d11cba50)
192:exercises_2025 eric$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   home.html
        new file:   team.html

Dropped stash@{0} (c824a572c88f4905cbcf7f0efd900b0552a0643d)
192:exercises_2025 eric$ git stash pop stash@{0}
stash@{0} is not a valid reference
192:exercises_2025 eric$ git stash
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash list
stash@{0}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash list
stash@{0}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash 
No local changes to save
192:exercises_2025 eric$ git status
On branch dev
nothing to commit, working tree clean
192:exercises_2025 eric$ git stash pop 
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   home.html
        new file:   team.html

Dropped refs/stash@{0} (d731e0cd3085e213178615bb55d9fbc8a4d79dc2)
192:exercises_2025 eric$ git stash
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git status
On branch dev
nothing to commit, working tree clean
192:exercises_2025 eric$ git stash pop
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   home.html
        new file:   team.html

Dropped refs/stash@{0} (c1478e46414d907f06304b28fa8e8119547dd171)
192:exercises_2025 eric$ git stash  About.html
usage: git stash list [<options>]
   or: git stash show [<stash>]
   or: git stash drop [-q|--quiet] [<stash>]
   or: git stash ( pop | apply ) [--index] [-q|--quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash save [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                      [-u|--include-untracked] [-a|--all] [<message>]
   or: git stash [push [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                       [-u|--include-untracked] [-a|--all] [-m <message>]
                       [-- <pathspec>...]]
   or: git stash clear
192:exercises_2025 eric$ git stash  About.html .
usage: git stash list [<options>]
   or: git stash show [<stash>]
   or: git stash drop [-q|--quiet] [<stash>]
   or: git stash ( pop | apply ) [--index] [-q|--quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash save [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                      [-u|--include-untracked] [-a|--all] [<message>]
   or: git stash [push [--patch] [-k|--[no-]keep-index] [-q|--quiet]
                       [-u|--include-untracked] [-a|--all] [-m <message>]
                       [-- <pathspec>...]]
   or: git stash clear
192:exercises_2025 eric$ git status
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   home.html
        new file:   team.html

192:exercises_2025 eric$ git stash
Saved working directory and index state WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git status
On branch dev
nothing to commit, working tree clean
192:exercises_2025 eric$ git stash pop  team.html
team.html is not a valid reference
192:exercises_2025 eric$ git stash pop  team.html
team.html is not a valid reference
192:exercises_2025 eric$ git stash list 
stash@{0}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash
No local changes to save
192:exercises_2025 eric$ git stash list
stash@{0}: WIP on dev: 4a004ae innitial commit
192:exercises_2025 eric$ git stash pop
On branch dev
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   About.html
        new file:   home.html
        new file:   team.html

Dropped refs/stash@{0} (836d05050a22cfb51b9aa5f85003dd8dca47c762)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$  git commit -m"second commit in git exercises"
[dev 6de86f2] second commit in git exercises
 3 files changed, 36 insertions(+)
 create mode 100644 About.html
 create mode 100644 home.html
 create mode 100644 team.html
192:exercises_2025 eric$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

192:exercises_2025 eric$     git push --set-upstream origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 669 bytes | 669.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   4a004ae..6de86f2  dev -> dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.
192:exercises_2025 eric$ git stash list
192:exercises_2025 eric$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git stash list 
192:exercises_2025 eric$ git status 
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tr
```