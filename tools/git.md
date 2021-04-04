# Git

- [Git](#git)
  - [Commands](#commands)
    - [Show git version](#show-git-version)
    - [Git clone project](#git-clone-project)
    - [Clone recursive (with submodules)](#clone-recursive-with-submodules)
    - [Git add all new files](#git-add-all-new-files)
    - [Git commit with message](#git-commit-with-message)
    - [Git push (Upload to gitlab)](#git-push-upload-to-gitlab)
    - [Git log (Show project history)](#git-log-show-project-history)
    - [Git status(List files changed)](#git-statuslist-files-changed)
    - [Git tag(Create an unmaintained version of your project)](#git-tagcreate-an-unmaintained-version-of-your-project)
    - [Git branch(Create a maintened version of a project)](#git-branchcreate-a-maintened-version-of-a-project)

## Commands

[GitHub](http://github.com)

---

### Show git version

```bash
git --version
```

### Git clone project

```bash
git clone <url>
```

### Git switch branch

```bash
git checkout <name of the branch>
```

### Clone recursive (with submodules)

```bash
git clone --recursive <url>
```

### Git add all new files

```bash
git add .
```

### Git commit with message

```bash
git commit -m "My horse is a toe"
```

### Git push (Upload to gitlab)

```bash
git push
```

### Git log (Show project history)

```bash
git log
```

### Git status(List files changed)

```bash
git status
```

### Git tag(Create an unmaintained version of your project)

```bash
git tag
```

### Git branch(Create a maintened version of a project)

```bash
git branch
```

### Git remote (Used to connect your repository to github)

```bash
git remote add [origin, main, etc] [https://github.com/myproject]
```