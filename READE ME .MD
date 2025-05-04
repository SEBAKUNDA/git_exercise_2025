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