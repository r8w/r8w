---
layout: default
parent: Tips & Tricks
grand_parent: notes.cs
title: YouTube
nav_order: 3
---

# YouTube
{: .no_toc}

*Everyday questions and answers!*

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

- ### How to download a playlist as mp3?

[`Ask Ubuntu`](https://askubuntu.com/questions/564567/how-to-download-playlist-to-mp3-format-with-youtube-dl)

```sh
$ youtube-dl --extract-audio --audio-format mp3 -o "%(title)s.%(ext)s" <url to playlist>
```

Add `playlist--start <index>` to start downloading from specific index.
