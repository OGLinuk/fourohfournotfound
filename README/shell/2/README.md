---
title: Shell 2 ~ Navigation
date: 2020-04-20T18:34:05+12:00
draft: false
tags: ["Shell,", "Linux,", "CLI,", "BASH,", "Open Source"]
---

Chapter 2 of [The Linux Command Line](http://www.linuxcommand.org/tlcl.php) covers *navigation*. The commands explored in this chapter are `pwd` (print working directory), `cd` (change directory), and `ls` (list directory contents). I use `cd` and `ls` daily, but I don't often use `pwd`. The structure of the Linux filesystem follows the [*Filesystem Hierarchy Standard (FHS)*](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard), meaning the filesystem is organized in a tree-like form of *directories*, which can contain files and other directories. The very base directory is called the *root directory*.

When working in the terminal emulator, we are always in a directory (usually somewhere in the *home* directory). This is called the *current working directory*. The current working directory can be viewed using the *print working directory* or `pwd` command. The contents of the current working directory can be viewed by using the *list directory contents* or `ls` command. An important note to remember about the `ls` command is that it is able to be used on *any* directory, not just the current working directory. To change the current working directory we use the *change directory* or `cd` command. The `cd` command is followed by the path to the target directory that you are wanting to change to. You can specify paths one of two ways; *relative* or *absolute*. 

*Relative* paths are just as the name suggests, pathnames that are *relative to the current working directory*. When working with relative paths there are two special notations that can be used to assist the pathing; `.` and `..`. The `.` notation refers to the current working directory, and the `..` notation refers to the *parent directory*. *Absolute* paths are pathnames to a location *regardless of the current working directory*. An absolute path starts with the root directory and follows the layout until the desired directory is reached. An example of an absolute path looks like `/etc/systemd/system`, where `system` would be the destination directory. 

Some important things to remember are first that *names are case sensitive* in Linux, so `/home/Desktop` will be a completely different directory than `/home/desktop`. Likewise with files, `hello.txt` will be a different file than `Hello.txt`. Second there are hidden files and directory that start with a `.`, such as `~/.ssh/` or `~/.bashrc`. Third Linux supports filenames and directories with spaces, but please *never embed spaces in names*. Save your sanity. Instead I suggest using an underscore or hyphen.  

Something that I learned from this chapter is `cd -`, which changes to the previous working directory. *Epic*.