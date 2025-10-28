#### To create an empty Git repository
- Navigate to your desired directory then type:
```bash 
git init
```

#### To download an existing Git repository
- Navigate to your desired directory then type:
```bash 
git clone "...."
```

### git clone [options]
Creates a local copy of a remote repository (downloads all files, branches, and history).

| `git clone [url]` | Clones a remote repository into a new local directory. | `git clone https://github.com/user/project.git` |
| ------------------ | -------------------------------- | ---- |
| `git clone [url] [folder-name]` | Clones the repository into a specific folder name. | `git clone https://github.com/user/project.git my-project` |
| `git clone -b [branch-name] [url]` | Clones a specific branch instead of the default one. | `git clone -b develop https://github.com/user/project.git` |
| `git clone --single-branch [url]` | Clones only the latest snapshot of a single branch (no full history). | `git clone --single-branch https://github.com/user/project.git` |
| `git clone --depth [n] [url]` | Creates a **shallow clone** with the last *n* commits (faster, smaller). | `git clone --depth 1 https://github.com/user/project.git` |
| `git clone --recurse-submodules [url]` | Clones the main repo **and all its submodules** recursively. | `git clone --recurse-submodules https://github.com/user/project.git` |