---
title: Script Executable
parent: Iteration 2
has_children: false
---

## Script Executable
A batch file is a script file in Microsoft Windows. It consists of a series of commands to be executed by the command-line interpreter, stored in a plain text file.

The interpreter executes each line in turn, starting with the first. The `@` symbol at the start of any line prevents the prompt from displaying that command as it is executed. The command `ECHO OFF` turns off the prompt permanently, or until it is turned on again. The combined `@ECHO OFF` is often as here the first line of a batch file, preventing any commands from displaying, itself included.

The ``PAUSE`` command displays ``Press any key to continue...`` and pauses the script's execution. After a key is pressed, the script terminates, as there are no more commands. In Windows, if the script is executed from an already running command prompt window, the window remains open at the prompt as in MS-DOS; otherwise, the window closes on termination.

**Example of _.bat_ file**
```
SET PATH = C:\Users\Public\Documents\;
START /d PATH Host.exe
ECHO Application started successfully
PAUSE
```