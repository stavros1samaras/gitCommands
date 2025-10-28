### git merge [branch]
Combines changes from another branch into the current branch.

| `git merge [branch-name]` | Merges the specified branch into the current branch. | `git merge feature/login-page` |
| --------------------------- | -------------------------------- | ---- |
| `git merge --ff-only [branch-name]` | Performs the merge **only** if it can be done with a fast-forward (no merge commit). | `git merge --ff-only hotfix/typo` |
| `git merge --abort` | Cancels an ongoing merge and restores the branch to its pre-merge state. | `git merge --abort` |
| `git merge -m "[message]" [branch-name]` | Adds a custom message to the merge commit. | `git merge -m "Merged feature branch" feature/api` |


# Examples and Best Practices
### Merging a feature branch into the main branch  (Fast-forward)

Pull the latest changes before merging:
```bash
git pull origin main
```
Perform merging:
```bash
git switch main
git merge feature/login-page
```
Output:
```bash
Updating a1b2c3d..d4e5f6g
Fast-forward
 login.js | 12 ++++++++++++
 1 file changed, 12 insertions(+)
```

### Merging using the recursive strategy (default non–fast-forward merge)
Pull the latest changes before merging
```bash
git pull origin main
```
Perform a non-fast-forward merge (recursive strategy is used by default)
```bash
git switch main
git merge feature/ui-update || git merge --no-ff feature/ui-update
```
During this process, Git will open your default text editor and ask you to enter a merge commit message, such as:
```bash
Merge branch 'feature/ui-update' into main
```
Output
```bash
Merge made by the 'recursive' strategy.
 ui.js | 8 ++++++++
 1 file changed, 8 insertions(+)
```
