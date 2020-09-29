- Skipping the Staging Area : `git commit -a` Shortcut to stage any changes to tracked files and commit them in one step.
- HEAD in Git Log : Git uses the head alias to represent the currently checked out snapshot of your project. Think about it as a bookmark that you can use to keep track of where you are. Even if you have multiple books to read, the bookmark allows you to pick up right where you left off.
- Getting more information about our changes:
  `git log` : History of commits
  `git log -p`: History of commits along with changes
  `git show commitid`: Show changes of a specific commitid
  `git log --stat`: Show log with some stat
  `git diff`: Show changes which are not yet staged
  `git add -p`: Ask confirmation before staging Files
  `git diff --staged`: Show changes which are staged
- Deleting, Renaming and Ignoring Files:
  `git rm fileNameToBeDeleted` : Deletes the specified file and adds it to the staging area which needs to be committed.
  `git mv oldFileName newFileName` : Rename file
  `git add .ignoreFile` : Add files to be ignored to this file
