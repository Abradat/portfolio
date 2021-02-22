---
layout: portfolio_detail_text
order: 14
title:  Linux Kernel Module
name: linux-kernel-module
badge-description: A kernel module for hooking read and write system calls and encryption using ROT13
filter: filter-os
badge-image: badge.jpg
category: OS
client:
project-date: Fall 2019
project-url:
github-repository: abradat/kernel-hook-module
full-description: A kernel module for hooking read and write system calls and encryption using ROT13
---
#### Introduction
This project is a module for hooking system calls at the kernel level. This module should encrypt inputs from user when **echo** and **tee** commands are called and decrypt them when **cat** command is called. **ROT13** algorithm is used for encryption.

**cat** command is used for reading the content of a file and printing as the output. Also, **echo** and **tee** commands are used for writing inputs. We can retrieve system calls in each command by utilizing **strace** command. In order to change the functionality of cat, echo, and tee commands, **read** and **write** system calls are hooked at kernel level and the encryption/decryption algorithm code is injected before these system calls are called.
#### Technologies/Languages Used

{: .table .table-striped}
| Technology | Usage |
|------------------|--------|
| <img src="{{'assets/img/portfolio/technologies/c.png' | relative_url}}" width="60" height="60"> | **C** is the main language being used in kernel development |
| <img src="{{'assets/img/portfolio/technologies/linux.png' | relative_url}}" width="60" height="60"> | All the development has been done on **Linux Kernel** |
| <img src="{{'assets/img/portfolio/technologies/git.png' | relative_url}}" width="60" height="60"> | **Git** is used for the version control. |