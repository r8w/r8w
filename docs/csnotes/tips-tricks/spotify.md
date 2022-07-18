---
layout: default
parent: Tips & Tricks
grand_parent: notes.cs
title: Spotify
nav_order: 4
---

# Spotify
{: .no_toc}

*Everyday questions and answers!*

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

- ### GPU Process isn't usable. Goodbye!

```
[0718/114001.865106:FATAL:gpu_data_manager_impl_private.cc(445)] GPU process isn't usable. Goodbye.
```

```sh
$ spotify --no-zygote
```

The source of this problem is a [bug](https://codereview.chromium.org/2384163002) present in Chromium, and Spotify Desktop Application is built upon chromium.

---

- ### Spotify Desktop -- Adblock

I use [Spotify Adblock](https://github.com/abba23/spotify-adblock) which works by wrapping `getaddrinfo` and `cef_urlrequest_create`. It blocks requests to domains that are not on the *allowlist*, as well as URLs that are on the *denylist*.
