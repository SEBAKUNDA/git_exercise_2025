#Git exercise project

This project will be used for series of git exercise

#bash1#
```bash

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  main
192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
192:exercises_2025 eric$  git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"new change "
[main 83b4feb] new change
 1 file changed, 1 insertion(+), 1 deletion(-)
192:exercises_2025 eric$ git push
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/git_exercise_2025.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git push
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/git_exercise_2025.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
192:exercises_2025 eric$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), done.
From https://github.com/SEBAKUNDA/git_exercise_2025
   4a004ae..5d0a04d  main       -> origin/main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 792 bytes | 792.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   5d0a04d..2b1e07d  main -> main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
192:exercises_2025 eric$ git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
* ft/home-page-redesign
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git pull --rebase
error: cannot pull with rebase: You have unstaged changes.
error: please commit or stash them.
192:exercises_2025 eric$ git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"rebasing"
[ft/home-page-redesign 85b6e6b] rebasing
 1 file changed, 1 insertion(+), 1 deletion(-)
192:exercises_2025 eric$ git pull --rebase
Current branch ft/home-page-redesign is up to date.
192:exercises_2025 eric$ git status
On branch ft/home-page-redesign
Your branch is ahead of 'origin/ft/home-page-redesign' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch ft/home-page-redesign
Your branch is ahead of 'origin/ft/home-page-redesign' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"commiting"
[ft/home-page-redesign edb8c4d] commiting
 1 file changed, 12 insertions(+)
 create mode 100644 home.html
192:exercises_2025 eric$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 603 bytes | 603.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   92a4706..edb8c4d  ft/home-page-redesign -> ft/home-page-redesign
192:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ 

```
```bash

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git init 
Reinitialized existing Git repository in /Users/eric/exercises_2025/.git/
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   team.html

192:exercises_2025 eric$ git commit -m"new commiting"
[main 762e36b] new commiting
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
192:exercises_2025 eric$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 512 bytes | 512.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   7d71a32..762e36b  main -> main
192:exercises_2025 eric$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
192:exercises_2025 eric$ git remote add origin https://github.com/SEBAKUNDA/ft-team-page.git
fatal: remote origin already exists.
192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
* ft/team-page
  main
Erics-MacBook-Pro:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Erics-MacBook-Pro:exercises_2025 eric$ git git add .
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init
Erics-MacBook-Pro:exercises_2025 eric$ git add .
Erics-MacBook-Pro:exercises_2025 eric$ git commit -m"after resolving"
[main 0eed253] after resolving
 1 file changed, 7 deletions(-)
Erics-MacBook-Pro:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   762e36b..0eed253  main -> main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ 
```
```bash
nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
* ft/team-page
  main
Erics-MacBook-Pro:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Erics-MacBook-Pro:exercises_2025 eric$ git git add .
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init
Erics-MacBook-Pro:exercises_2025 eric$ git add .
Erics-MacBook-Pro:exercises_2025 eric$ git commit -m"after resolving"
[main 0eed253] after resolving
 1 file changed, 7 deletions(-)
Erics-MacBook-Pro:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   762e36b..0eed253  main -> main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   READE ME .MD

no changes added to commit (use "git add" and/or "git commit -a")
Erics-MacBook-Pro:exercises_2025 eric$ git add .
Erics-MacBook-Pro:exercises_2025 eric$ git commit -m"read me"
[main ad99e5a] read me
 1 file changed, 108 insertions(+)
Erics-MacBook-Pro:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1014 bytes | 1014.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   0eed253..ad99e5a  main -> main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ 
 *  History restored 


The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git status
On branch main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
192:exercises_2025 eric$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ pwd
/Users/eric/exercises_2025
192:exercises_2025 eric$ git remote add https://github.com/SEBAKUNDA/GitRep.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

192:exercises_2025 eric$ git remote add git-copy https://github.com/SEBAKUNDA/GitRep.git
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"commiting"
[main f9187f2] commiting
 1 file changed, 12 insertions(+)
 create mode 100644 home.html
192:exercises_2025 eric$ git remote -v
git-copy        https://github.com/SEBAKUNDA/GitRep.git (fetch)
git-copy        https://github.com/SEBAKUNDA/GitRep.git (push)
origin  https://github.com/SEBAKUNDA/git_exercise_2025.git (fetch)
origin  https://github.com/SEBAKUNDA/git_exercise_2025.git (push)
192:exercises_2025 eric$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 525 bytes | 525.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   ad99e5a..f9187f2  main -> main
192:exercises_2025 eric$ git push git-copy main
Enumerating objects: 39, done.
Counting objects: 100% (39/39), done.
Delta compression using up to 8 threads
Compressing objects: 100% (35/35), done.
Writing objects: 100% (39/39), 6.43 KiB | 1.61 MiB/s, done.
Total 39 (delta 11), reused 0 (delta 0)
remote: Resolving deltas: 100% (11/11), done.
To https://github.com/SEBAKUNDA/GitRep.git
 * [new branch]      main -> main
192:exercises_2025 eric$ 
```
```bash
nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
* ft/team-page
  main
Erics-MacBook-Pro:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
Erics-MacBook-Pro:exercises_2025 eric$ git git add .
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init
Erics-MacBook-Pro:exercises_2025 eric$ git add .
Erics-MacBook-Pro:exercises_2025 eric$ git commit -m"after resolving"
[main 0eed253] after resolving
 1 file changed, 7 deletions(-)
Erics-MacBook-Pro:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   762e36b..0eed253  main -> main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   READE ME .MD

no changes added to commit (use "git add" and/or "git commit -a")
Erics-MacBook-Pro:exercises_2025 eric$ git add .
Erics-MacBook-Pro:exercises_2025 eric$ git commit -m"read me"
[main ad99e5a] read me
 1 file changed, 108 insertions(+)
Erics-MacBook-Pro:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1014 bytes | 1014.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   0eed253..ad99e5a  main -> main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
Erics-MacBook-Pro:exercises_2025 eric$ 
 *  History restored 


The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git status
On branch main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch
192:exercises_2025 eric$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ pwd
/Users/eric/exercises_2025
192:exercises_2025 eric$ git remote add https://github.com/SEBAKUNDA/GitRep.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

192:exercises_2025 eric$ git remote add git-copy https://github.com/SEBAKUNDA/GitRep.git
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"commiting"
[main f9187f2] commiting
 1 file changed, 12 insertions(+)
 create mode 100644 home.html
192:exercises_2025 eric$ git remote -v
git-copy        https://github.com/SEBAKUNDA/GitRep.git (fetch)
git-copy        https://github.com/SEBAKUNDA/GitRep.git (push)
origin  https://github.com/SEBAKUNDA/git_exercise_2025.git (fetch)
origin  https://github.com/SEBAKUNDA/git_exercise_2025.git (push)
192:exercises_2025 eric$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 525 bytes | 525.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   ad99e5a..f9187f2  main -> main
192:exercises_2025 eric$ git push git-copy main
Enumerating objects: 39, done.
Counting objects: 100% (39/39), done.
Delta compression using up to 8 threads
Compressing objects: 100% (35/35), done.
Writing objects: 100% (39/39), 6.43 KiB | 1.61 MiB/s, done.
Total 39 (delta 11), reused 0 (delta 0)
remote: Resolving deltas: 100% (11/11), done.
To https://github.com/SEBAKUNDA/GitRep.git
 * [new branch]      main -> main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   READE ME .MD

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"readME bash"
[main 2b41fc1] readME bash
 1 file changed, 209 insertions(+)
192:exercises_2025 eric$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.01 KiB | 1.01 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   f9187f2..2b41fc1  main -> main
192:exercises_2025 eric$ git branch --show-current
error: unknown option `show-current'
usage: git branch [<options>] [-r | -a] [--merged | --no-merged]
   or: git branch [<options>] [-l] [-f] <branch-name> [<start-point>]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track           set up tracking mode (see git-pull(1))
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      Unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display SHA-1s

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --format <format>     format to use for the output

192:exercises_2025 eric$ cat .git/HEAD
ref: refs/heads/main
192:exercises_2025 eric$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ cat .git/HEAD
ref: refs/heads/main
192:exercises_2025 eric$ 
```