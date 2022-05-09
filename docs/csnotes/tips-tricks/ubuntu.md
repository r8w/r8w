---
layout: default
parent: Tips & Tricks
grand_parent: notes.cs
title: Ubuntu
nav_order: 2
---

# Ubuntu
{: .no_toc}

*Everyday questions and answers!*

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

- ### How to flush DNS Cache in Ubuntu 16.04

[`Linux Hint`](https://linuxhint.com/flush_dns_cache_ubuntu/) -- [`Dream Host`](https://help.dreamhost.com/hc/en-us/articles/214981288-Flushing-your-DNS-cache-in-Mac-OS-X-and-Linux)

```sh
$ sudo systemd-resolve --statistics
$ sudo systemd-resolve --flush-caches
$ sudo systemctl restart systemd-resolved
# or
$ sudo systemctl restart nscd
```
---

