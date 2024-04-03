---
marp: true
theme: uncover
paginate: true
---

# Git advanced

### First workshop

by [@condef5](https://twitter.com/condef5)

---

### Git clone

Clone this repository https://github.com/Bootcamp-x/recetas-selvaticas

---

### Git log

```sh
git log
git log --oneline
git log -n 5
```

---

### Git blame

```sh
git blame filename
```

For vscode users, use [git lens extension](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)

---

# Git remote

```sh
git remote -v
```

---

### Create a new remote

```sh
git remote add [remote-name] [url repository]
```

---

### Delete a remote

```sh
git remote remove [remote-name]
```

---

### Git branch

```sh
git branch branch-name
```

---

### Git checkout

```sh
git checkout branch-name
```

---

# Git add

```sh
git add .
```

---

```sh
git add -p filename
```

---

### First Task

1. In groups of 2 people, create a new branch.
2. Each member should add a commit from their computer.
3. Upload your changes.
4. Create a unique pull request per group.
5. Merge the pull request from GitHub.
6. Update your local branches.

---

### Good Commits

1. Brief and descriptive: The commit message should be brief yet descriptive, clearly and concisely
2. Use imperatives: Commit messages should start with an imperative verb, such as "Add", "Fix", "Update", "Remove", etc.
3. Proper capitalization and punctuation.
4. Keep it reasonably short.
5. Reference to issues or pull requests.

---

### Commit Conventions

---

### Fix (Corrección):

It is used when a commit resolves an error or bug in the code.
It is useful to quickly identify commits that fix specific issues in the code.
Example commit message: `Fix issue with login form validation`

---

### Chore:

It is used for changes that are not directly related to user functionality or error correction, such as administrative tasks, refactoring, dependency updates, etc.

It helps separate functional changes from other types of changes in the repository history.
Example commit message: `Update dependencies`

---

### Feat (Característica):

It is used to indicate the implementation of a new feature or functionality in the code.

It is useful to quickly identify commits that add new features to the project.

Example commit message: `Add user profile page`

---

### Second Task

1. Repeat task 1 using good commits and commit conventions

---

### Git commit

```sh
git commit
git commit -m 'message'
git commit --allow-empty -m "Trigger Build"
```

---

# Git stash

```sh
git stash
```

> When you run git stash, Git saves uncommitted changes to a temporary storage area called "stash."
> This leaves your working directory clean so you can switch branches, apply patches, merge changes, etc.

---

List all stash

```sh
  git stash list
```

Apply last stash saved

```sh
  git stash apply
```

---

Applies the changes from the stash specified by the index n in the stash list.

```sh
  git stash apply stash@{n}
```

---

### Third Task

1. Create a commit to references some link
2. Save some changes using stash
3. Use stash apply
4. Create 3 stash and apply the second one.

---

# Git merge

---

# Git rebase

---

# Git rebase onto

```sh
 git rebase --onto branch-name head~n

 # example
 git rebase --onto dev head~3
```

---

# Git reset

```sh
git reset
git reset --soft head~1
```

---

```sh
git commit --amend --no-edit
```

---

# Git reflog

```sh
git reflog
```

---
