---
title: What is Shell?
date: 2020-04-19T01:09:38+12:00
draft: false
tags: ["Shell,", "Linux,", "CLI,", "BASH,", "Open Source"]
---

If you are using a debian based Linux distribution like I am, then the shell you are using whats called *BASH* or "Bourne Again SHell", which is a GNU project created by [Brian Fox](https://en.wikipedia.org/wiki/Brian_Fox_(computer_programmer)). Another amazing human being. If you ever happen to read this blog Brian, thank you. To interact with the shell we use another program called a *terminal emulator*, which in my case is [alacritty](https://github.com/alacritty/alacritty) (thanks to [rwxrob](https://gitlab.com/rwxrob) for showing me and the 276 current people working on it). To open the terminal emulator you can use the shortcut `ctrl + alt + t`. An interesting note that the book makes is that if the last character of the shell prompt is a `#` sign rather than a `$` sign, then the session has *superuser* privileges. Only two pages into the first chapter and already learning something new. 

If we have already typed commands into the shell prompt then we will have access to the *command history* which is accessible via the up-arrow and down-arrow keys. The book states that even the mouse is capable of interacting with the terminal emulator via the [X Window System](https://en.wikipedia.org/wiki/X_Window_System). If you highlight text by holding down the left mouse button and dragging the mouse over it (or double clicking a word), it is copied into a buffer maintained by X. This can then be pasted with the middle mouse button. Wow. I've always used `ctrl + shift + c/v` with the highlighted text, I never realized it was copied when it's highlighted, nor that you can paste with middle mouse button.

Now for some basic commands. The first is `date`, which as you might guess, displays the current datetime. The second is `cal` which displays a calendar. The third is `df` which shows the amount of free space on the disk drives. The fourth is `free` which displays the amount of free memory. Of these, the only one I knew about is `df`, which I use with the `-h` flag to make the output human readable. To end the terminal session you can either type `exit` or enter the shortcut (which I never knew about until now) `ctrl + d`.

I want to just give a tip to anyone who might be like me and be too eager to try things before reading something entirely. ***Don't***. Read the entire section before doing something or you will end up in panic mode like I just was cause I executed `ctrl + alt + f1` and entered into a virtual terminal without knowing how to get back to the graphical desktop (`alt + f7`). There are up to six virtual terminals accessible via `ctrl + alt + f1-6`. 

Already learning so much and that was only from the first chapter!