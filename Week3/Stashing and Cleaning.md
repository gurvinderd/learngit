## Stashing and Cleaning
- [Git Tools - Stashing and Cleaning](https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning#_git_stashing)
- Stashing takes the dirty state of your working directory — that is, your modified tracked files and staged changes — and saves it on a stack of unfinished changes that you can reapply at any time (even on a different branch)
- `git status` : Start working on a couple of files and possibly stage one of the changes
- `git stash` or `git stash push` : To push a new stash onto your stack
- `git status` : You can now see that your working directory is clean
- `git stash list` : To see which stashes you’ve stored
- `git stash apply` : You can reapply the one you just stashed
- `git stash apply stash@{2}` : If you want to apply one of the older stashes, you can specify it by naming it
- `git stash apply --index` : Apply the changes and reapply the staged changes
- `git stash drop stash@{0}` : To remove it, you can run git stash drop with the name of the stash to remove
- `git stash pop` : To apply the stash and then immediately drop it from your stack

## Creative Stashing
- `git status -s`
- `git stash --keep-index` : This tells Git to not only include all staged content in the stash being created, but simultaneously leave it in the index
- `git status -s`
- `git stash -u` or `git stash --include-untracked` : Git will include untracked files and tracked files in the stash being created
- `git status -s`

## Creating new branch from Stash
- `git stash branch <new branchname>` : Creates a new branch for you with your selected branch name, checks out the commit you were on when you stashed your work, reapplies your work there, and then drops the stash if it applies successfully


## Cleaning
- `git clean` : Remove files from your working directory that are not tracked
- `git stash --all` : Remove everything but save it in a stash
- `git clean -f -d` :  Removes any files and also any subdirectories that become empty as a result
- `git clean -d -n` OR `git clean -d --dry-run` : Do a dry run and tell me what you would have removed
- `git status -s`
