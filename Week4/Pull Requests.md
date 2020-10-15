## Squashing changes
- [Rewriting History](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History)
- `git rebase -i master`
- `squash`
- `git show`
- `git status`
- `git log --graph --oneline --all 4`
- `git push`
- `git push -f`

## Address Review comments
- `git commit -a --amend`
- `git push -f`
- [Google Style Guide](https://google.github.io/styleguide/)
- [Google Engineering Practices](https://github.com/google/eng-practices)
-  Nit : Reviewers should always feel free to leave comments expressing that something could be better, but if it’s not very important, prefix it with something like “Nit: “ to let the author know that it’s just a point of polish that they could choose to ignore
-  Nit : https://google.github.io/eng-practices/review/reviewer/standard.html#:~:text=Reviewers%20should%20always%20feel%20free,they%20could%20choose%20to%20ignore.
- ChangeLog : https://google.github.io/eng-practices/review/developer/cl-descriptions.html
