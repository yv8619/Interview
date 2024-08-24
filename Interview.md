# GIT

## What is the difference between git fetch and git pull?
‘git fetch’ fetches updates from a remote repository but does not combine them into your local repository. 
‘git pull‘ fetches the updates from the remote repository and instantly strives to merge them into your current branch. 
git pull = git fetch + git merge

## what is git rebase ?
Git rebase is a way to take changes you've made on one branch and put them on top of another branch, making the history of your work look neat and linear.

## diff btw merging and rebasing ?
Merging: Combines the changes from two branches by creating a new "merge commit" that has two parent commits, one from each branch.
Rebasing: Instead of creating a merge commit, it moves (or reapplies) the commits from one branch onto another, making the history linear.

## What is git stash?
Git stash is a feature in Git that allows you to temporarily save (or "stash away") your changes that are not yet committed, so you can switch to another task, like working on a different branch, 
without losing your work. After you've finished the other task, you can come back and apply (or "unstash") those changes.

## Difference Between Git Push Origin and Git Push Origin Master ?
Git Push Origin - is used to push your current branch to the remote repository named origin. However, this command requires an upstream branch to be set for the current branch.
git push --set-upstream origin your-branch-name
Git Push Origin Master - Git Push Origin Master pushes your master branch to the origin.

## How to Fix “master branch and ‘origin/master’ have diverged”?
arises when:
Local Changes: You’ve made commits on your local master branch that are not present on the remote origin/master.
Remote Changes: The remote origin/master branch has new commits that are not present on your local master.
To resolve this issue, you must reconcile these differences, ensuring that both branches reflect a consistent history.

## how to Create a New Branch from a Specific Commit ?
git checkout -b new-branch-name commit#
git checkout -b new-branch-name origin/remote-branch-name ( creating branch from a remote branch )

## how to delete branch locally and on remote ?
git branch -d yvtest
git push origin --delete yvtest

## how to rename a branch ?
git branch -m yvtest yvtest1




 


