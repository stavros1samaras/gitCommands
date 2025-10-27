### git add [options]
Adds file contents to the staging area (index).

| `git add [filename]` | Adds a specific file to the staging area. | `git add index.html` |
| --------------------- | -------------------------------- | ---- |
| `git add .` | Adds **all modified and new files** in the current directory. | `git add .` |
| `git add -p` | Interactively stages parts (hunks) of a file. | `git add -p` |

---

### git commit [options]
Records changes to the repository.

| `git commit -m "[message]"` | Creates a new commit with a message. | `git commit -m "Initial commit"` |
| ---------------------------- | -------------------------------- | ---- |
| `git commit -am "[message]"` | Stages and commits all modified tracked files (skips `git add`). | `git commit -am "Update styles"` |
| `git commit --amend` | Modifies the most recent commit (message or files). | `git commit --amend -m "Fix typo"` |
