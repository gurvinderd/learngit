## Pull Merge Push Workflow
- `git add -p` : Ask confirmation before staging Files
- `git commit -m 'commit message goes here'`
- `git push` : Push changes to remote
- `git pull` : Fetch and Merge changes from origin, should show merge conflicts if fast forward merge doesn't work. Three way merge would be required.
- `git log --graph --oneline --all`
- `git log -p origin/master`
- `git add FileName`
- `git commit -m 'commit message'`
- `git push`
- `git log --graph --oneline`

## Pushing Remote Branches
- `git checkout -b newfeature` : Create and switch to new branch
- `git commit -a -m 'commit message'` : Stage and commit new changes, this can stage existing files not the new files.
- `git push -u origin newfeature` : Create new remote branch and push

## Rebasing your Changes
- Rebasing means changing the base commit that's used for our branch
- Below we will Rebase with master
- `git checkout master` : Switch to master
- `git pull` : Pull latest master from remote
- `git log --graph --oneline --all` : Check log
- `git checkout newfeaturebranch` : Checkout feature branch
- `git rebase master` : Rebase current checkedout feature branch with master
- `git checkout master` : Switch to master
- `git merge newfeaturebranch` : Merge to master
- `git push --delete origin newfeaturebranch` : Delete remote feature
- `git branch -d newfeaturebranch` : Delete local feature
- `git push` : Push to remote

## Another Rebasing Example
- `git commit -a -m "commit message"`
- `git checkout master`
- `git fetch` : Fetch from remote
- `git rebase origin/master` : Rebase with remote master
- `git add fileName`
- `git rebase --continue`
- `git push`

## CheatSheet & Tips
- `git commit --amend --no-edit` : Update content without changing last commit message
- https://www.coursera.org/learn/introduction-git-github/supplement/bnibQ/conflict-resolution-cheat-sheet
- https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-merge-conflicts
- https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/resolving-a-merge-conflict-using-the-command-line
- https://git-scm.com/book/en/v2/Git-Branching-Rebasing
- https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History
