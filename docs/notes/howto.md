---
layout: default
parent: Notes
title: How To
nav_order: 0
---

# How To
{: .no_toc }

Everyday questions and answers!

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


---

# Git

 - [How to show only modified file using git?](https://stackoverflow.com/questions/10018533/is-it-possible-to-git-status-only-modified-files)

 ```sh
 $ git status -uno -sb
 ```

---

- [Reverting to specific commit in git and push it.](https://stackoverflow.com/questions/3639115/reverting-to-a-specific-commit-based-on-commit-id-with-git)

```sh
$ git reset SHA

$ git push -u origin master --force
```
---

- [Temporarily ignore changed or new files without altering `.gitignore`](https://gist.github.com/sloanlance/0f0cb5e9819e11d698a26a623bc649f4)

If the file is a changed repository file:

```sh
git update-index --assume-unchanged "$FILE"
````

To undo this, use the command:

```sh
git update-index --no-assume-unchanged "$FILE"
````

The update-index command doesn't work with new files that haven't been added to the repository yet, though.

If the file is new and not added to the repository:

Add its filename to the repository's exclude file:

```sh
echo "$FILE" >> .git/info/exclude
```

This also works for changed repository files, but there isn't a specific undo command for it. The exclude file would need to be edited and the filename deleted from it. Or other commands could approximate it:

```sh
ex -s -c"g/^${FILE}\$/d" -cwq .git/info/exclude
```
__Further__

- [Ignore trivial changes to files](https://stackoverflow.com/questions/13442130/git-temporarily-ignore-trivial-changes-to-files)

---

