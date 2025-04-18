﻿Lab 2 Repo
# 2nd-repo


## How to remove branches locally and remotely 


**git branch -d branch-name** : this deletes the branch locally if it's merged.

**git branch -D branch-name** : this deletes the branch locally if it's not merged.

**git push origin --delete branch-name** : this removes the branch from the remote repository.

## Git Tags

- **Annotated Tags**: Store metadata like the tagger’s name, message, and date.
- **Lightweight Tags**: Just a name pointing to a commit without extra info.

## When to use Rebase

**git rebase** is used to replay your changes on top of another branch, making your Git history cleaner and more linear. It’s super handy in collaborative work.

**Use rebase when:**

**1.You’re syncing your branch with main before merging:**

- Keeps history clean and avoids unnecessary merge commits.

**Example:**

- bash
- Copy
- Edit
- git checkout feature-branch
- git fetch origin
- git rebase origin/main
- You want to squash commits together:

**2-Ideal for cleaning up before pushing or opening a pull request.**

**Example:**

- bash
- Copy
- Edit
- git rebase -i HEAD~3  => Squash the last 3 commits

**3-You want a linear history:**

- Makes git log easier to read and avoids messy merge graphs.

## How to List Tags in Git :

**To view all tags in your repo:**

- bash
- Copy
- Edit
- git tag

**You’ll get a list like:**

- Copy
- Edit
- v1.0
- v1.7
- v2.0

## How to delete a tag locally and remotely

**delete a tag locally :** git tag -d v1.7

**delete a tag remotely:** git push origin --delete tag v1.7


![ITI Logo](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9afXVML2UMaMFwb3fzaIxlIxIlm2EkVefeQ&s)






