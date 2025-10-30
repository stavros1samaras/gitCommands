

### git stash [options]
Temporarily saves (stashes) uncommitted changes so you can work on something else without committing.

| `git stash` | Saves current uncommitted changes (both staged and unstaged). | `git stash` |
| ------------ | -------------------------------- | ---- |
| `git stash list` | Shows all stashed changes. | `git stash list` |
| `git stash apply` | Reapplies the most recent stash without removing it from the stash list. | `git stash apply` |
| `git stash pop` | Reapplies the most recent stash **and removes it** from the stash list. | `git stash pop` |
| `git stash drop` | Deletes the most recent stash without applying it. | `git stash drop` |
| `git stash clear` | Deletes **all** stashes. | `git stash clear` |
| `git stash show -p` | Shows the detailed changes of the most recent stash (patch). | `git stash show -p` |
| `git stash branch [branch-name]` | Creates a new branch from the stash and applies it there. | `git stash branch fix-bug` |
