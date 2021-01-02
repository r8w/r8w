---
layout: default
parent: Notes
title: How To
nav_order: 0
---

# How To
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


# Markdown

- Open link in a new tab

`[URL](LINK){:target="_blank"}`

# Git

- *.gitignore* unable to ignore files - [Stackoverflow](https://stackoverflow.com/questions/26238157/git-still-shows-files-as-untracked-despite-gitignore-and-rm-r-cached-what-d)

Best case - Change encoding of *.gitignore* to __UTF-8__ without *BOM*

```
$ gedit --encoding=UTF-8 filename
```

