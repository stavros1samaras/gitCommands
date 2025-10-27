### git branch [options]
Manages branches in a Git repository (create, list, delete, or rename branches).

| `git branch` | Lists all local branches in the repository. | `git branch` |
| ------------- | -------------------------------- | ---- |
| `git branch [branch-name]` | Creates a new branch with the specified name. | `git branch feature-login` |
| `git branch -d [branch-name]` | Deletes a branch (only if it has been merged). | `git branch -d old-feature` |
| `git branch -D [branch-name]` | Force deletes a branch, even if not merged. | `git branch -D test-branch` |
| `git branch -m [new-name]` | Renames the current branch to the new name. | `git branch -m main` |
| `git branch -a` | Lists both local and remote branches. | `git branch -a` |
| `git branch -r` | Lists only remote branches. | `git branch -r` |