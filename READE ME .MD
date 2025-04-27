#Git exercise project

This project will be used for series of git exercise

#bash1#
```bash
192:exercises_2025 eric$  git status
On branch ft/bundle2
Your branch is up to date with 'origin/ft/bundle2'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
* ft/bundle2
  main
192:exercises_2025 eric$  git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ fit branch 
bash: fit: command not found
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
* main
192:exercises_2025 eric$ git pull
Already up to date.
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git pull origin main
From https://github.com/SEBAKUNDA/git_exercise_2025
 * branch            main       -> FETCH_HEAD
Already up to date.
192:exercises_2025 eric$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
* ft/service-redesign
  main
192:exercises_2025 eric$ git status
On branch ft/service-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        services.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add      services.html
192:exercises_2025 eric$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   services.html

192:exercises_2025 eric$ git commit -m"new change in services"
[ft/service-redesign 7fdcb71] new change in services
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
192:exercises_2025 eric$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

192:exercises_2025 eric$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 506 bytes | 506.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/git_exercise_2025/pull/new/ft/service-redesign
remote: 
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
192:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/service-redesign
* main
192:exercises_2025 eric$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        services.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git push
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/SEBAKUNDA/git_exercise_2025.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"in main branch"
[main 1caab08] in main branch
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
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
Your branch is ahead of 'origin/main' by 1 commit.
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
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"changes"
[main 9d32370] changes
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
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
192:exercises_2025 eric$ git status
On branch ft/team-page
nothing to commit, working tree clean
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/service-redesign
* ft/team-page

```