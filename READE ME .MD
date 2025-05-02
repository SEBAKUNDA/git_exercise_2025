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
#exercices3
``` bash

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
192:exercises_2025 eric$ git status
192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        team.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"changes on team file"
[ft/team-page 9933ed9] changes on team file
 1 file changed, 13 insertions(+)
 create mode 100644 team.html
192:exercises_2025 eric$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 527 bytes | 527.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   512801d..9933ed9  ft/team-page -> ft/team-page
192:exercises_2025 eric$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
  ft/service-redesign
  ft/team-page
* main
192:exercises_2025 eric$ git branch -b ft/contact-page
error: unknown switch `b'
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

192:exercises_2025 eric$ git branch checkout -b ft/contact-page
error: unknown switch `b'
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

192:exercises_2025 eric$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
192:exercises_2025 eric$ hit log
bash: hit: command not found
192:exercises_2025 eric$ git log-1
git: 'log-1' is not a git command. See 'git --help'.
192:exercises_2025 eric$ git log
commit 9933ed948341efff3623e656ca18b1645f047fe8 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Fri May 2 00:00:05 2025 -0700

    changes on team file

commit 512801dc44614ca9545cfac6a8207dbac84ec8b3
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 04:33:41 2025 -0700

...skipping...












HELP -- Press RETURN for more, or q when done...skipping...
commit 9933ed948341efff3623e656ca18b1645f047fe8 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Fri May 2 00:00:05 2025 -0700

    changes on team file

commit 512801dc44614ca9545cfac6a8207dbac84ec8b3
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 04:33:41 2025 -0700

    commiting

commit 9d3237067fa7421956963545484a378f2fefe4d0 (main, ft/contact-page)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 03:36:56 2025 -0700

    changes

commit 1caab086941c81fdf00dd757c92ab861e0510089
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 03:35:19 2025 -0700

    in main branch

commit 4a004ae5a85744448e2dca579f5fa90187dcf406 (origin/main)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Wed Apr 23 12:45:49 2025 -0700

    innitial commit
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 03:35:19 2025 -0700

    in main branch

commit 4a004ae5a85744448e2dca579f5fa90187dcf406 (origin/main)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Wed Apr 23 12:45:49 2025 -0700

    innitial commit

192:exercises_2025 eric$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
192:exercises_2025 eric$ git branch
  dev
  ft/bundle2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git checkoutft/team-page
git: 'checkoutft/team-page' is not a git command. See 'git --help'.
192:exercises_2025 eric$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git branch 
  dev
  ft/bundle2
  ft/contact-page
  ft/service-redesign
* ft/team-page
  main
192:exercises_2025 eric$ git log 
commit 9933ed948341efff3623e656ca18b1645f047fe8 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Fri May 2 00:00:05 2025 -0700

    changes on team file

commit 512801dc44614ca9545cfac6a8207dbac84ec8b3
Author: Eric Sebakunda <esebakunda@gmail.com>
Date:   Sun Apr 27 04:33:41 2025 -0700

192:exercises_2025 eric$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
192:exercises_2025 eric$ git cherry pick  9933ed948341efff3623e656ca18b1645f047fe8
fatal: Unknown commit pick
192:exercises_2025 eric$ git cherry-pick  9933ed948341efff3623e656ca18b1645f047fe8
[ft/contact-page 38d140d] changes on team file
 Date: Fri May 2 00:00:05 2025 -0700
 1 file changed, 13 insertions(+)
 create mode 100644 team.html
192:exercises_2025 eric$ git branch 
  dev
  ft/bundle2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
192:exercises_2025 eric$ git branch 
  dev
  ft/bundle2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        fraq.html

nothing added to commit but untracked files present (use "git add" to track)
192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"new files of pages"
[ft/faq-page 754052a] new files of pages
 1 file changed, 12 insertions(+)
 create mode 100644 fraq.html
192:exercises_2025 eric$ git push 
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

192:exercises_2025 eric$  git push --set-upstream origin ft/faq-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 789 bytes | 789.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), done.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/SEBAKUNDA/git_exercise_2025/pull/new/ft/faq-page
remote: 
To https://github.com/SEBAKUNDA/git_exercise_2025.git
 * [new branch]      ft/faq-page -> ft/faq-page
Branch 'ft/faq-page' set up to track remote branch 'ft/faq-page' from 'origin'.
192:exercises_2025 eric$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

nothing to commit, working tree clean
192:exercises_2025 eric$ git revert 9933ed948341efff3623e656ca18b1645f047fe8 
hint: Waiting for your editor to close the file... error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.
192:exercises_2025 eric$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    team.html

192:exercises_2025 eric$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    team.html

192:exercises_2025 eric$ git branch 
  dev
  ft/bundle2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git revert 9933ed948341efff3623e656ca18b1645f047fe8 
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
192:exercises_2025 eric$ git branch 
  dev
  ft/bundle2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
192:exercises_2025 eric$ git checkout  ft/team-page
D       team.html
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
192:exercises_2025 eric$ git revert 9933ed948341efff3623e656ca18b1645f047fe8 
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed
192:exercises_2025 eric$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        deleted:    team.html

192:exercises_2025 eric$ git add .
192:exercises_2025 eric$ git commit -m"comming"
[ft/team-page 8b4d687] comming
 1 file changed, 13 deletions(-)
 delete mode 100644 team.html
192:exercises_2025 eric$ git revert 9933ed948341efff3623e656ca18b1645f047fe8 
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
192:exercises_2025 eric$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 217 bytes | 217.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/SEBAKUNDA/git_exercise_2025.git
   9933ed9..8b4d687  ft/team-page -> ft/team-page
192:exercises_2025 eric$ 
```