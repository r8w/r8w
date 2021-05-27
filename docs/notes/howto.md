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

- [Reverting to specific commit in git and push it.](https://stackoverflow.com/questions/3639115/reverting-to-a-specific-commit-based-on-commit-id-with-git)

```sh
$ git reset SHA

$ git push -u origin master --force
```
