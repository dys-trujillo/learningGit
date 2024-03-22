Code created to learn about git, using IntelliJ to test modifications and git integration. It is a functional code tho.

As a study roadmap:

git status: verify which files were changed

To register a change:

1. git add: add changes in order to commit

2. git commit: register changes in repo (use -m + "message" to include title)

3. git push: upload changes into repo

To update branches and repo:

1. git pull: download changes from others/changes made directly in github

To undo a git commit, but not git pushed:

1. git reset --hard + previous commit: if not uploaded to remote branch, it is recommended to delete the commit and rewind to the second latest. Otherwise, version change will be impacted and not recommended for group coding
2. git reset --soft + previous commit hash: same as follows, but keep modifications in work directory.

To modify a commit:

1. git commit --amend -m "correct message"

To undo a git commit already pushed to remote:

1. git revert <commit hash>: will revert all changes made to this commit, not excluding history.
2. git revert -n <latest hash to keep>: will revert all commits until commit specified, not excluding history.
- After using git revert, you need to commit again to apply version reverted.

To see all commits and its states:

1. git log: shows all history of commits, local and remote.

