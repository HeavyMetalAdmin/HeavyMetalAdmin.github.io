---
date: 2019-10-22 10:00:00
title: Linux(bash) Shell Overview
categories:
  - Bash
  - Linux
  - Commands
description: Overview of Bash / Shell Commands.
type: Document
tags: [Bash,Linux,Commands]
---

### Linux Shell commands & scripting Overview\\Outline

#### Shell commands:

* ls
* pwd
* mkdir
* cp
* mv
* rm
* cd
* cat
* more
* head
* tail
* ls -a
* ls -l
* vi or nano
* grep
* using pipes “\|” with linux shell command
* Pause processes in the terminal
  * ^z
* Put process to background:
  * ^z, bg
* man
* view\\manage processes:
  * ps
  * top
  * kill
* change file permissions:
  * chmod

#### Useful control codes in the console\\terminal:

^Z (pause the running foreground process)

^D (“simulated” end of file)

^C “break” – attempt to halt running process

\#\!\\bin\\bash (that’s always the first line of a bash shell script)

Make executable with chmod:

chmod +x myscript

#### Variables:

$whatever

#### Predefined variables:

$path

#### List of folders where bash will look for commands:

Startup Scripts

* .profile

Setup\\change user environment on login

* .bashrc