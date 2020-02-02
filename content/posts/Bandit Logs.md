+++
title = "Bandit Logs"
date = "2020-31-01"
author = "Nik"
description = "This is my logs for OvertheWire Bandit wargames."
+++

#### Level 0
> Used commands:

	ssh bandit0@bandit.labs.overthewire.org -p 2220
	password: bandit0

#### Level 0 - 1

> Password is in the readme file in home directory

	ls #while ssh'd into bandit0
	exit
	ssh bandit1@bandit.labs.overthewire.org -p 2220
	password: boJ9jbbUNNfktd78OOpsqOltutMc3MY1

#### Level 1 - 2

> The password for the next level is stored in a file called - located in the home directory
>
>Used link: https://unix.stackexchange.com/questions/16357/usage-of-dash-in-place-of-a-filename

	ls
	cat ./-
	ssh bandit2@bandit.labs.overthewire.org -p 2220
	password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9 

#### Level 2-3

> The password for the next level is stored in a file called **spaces in this filename** located in the home directory

	ls
	cat "spaces in this filename"
	ssh bandit3@bandit.labs.overthewire.org -p 2220
	password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

#### Level 3-4

> The password for the next level is stored in a hidden file in the **inhere** directory
>
> Used [https://www.lostsaloon.com/technology/how-to-show-hidden-files-in-linux/](https://www.lostsaloon.com/technology/how-to-show-hidden-files-in-linux/)  to figure out how to find hidden files and the syntax for using cat on them
>
> ![lvl3-4.png](/banditimg/lvl3-4.png)

#### Level 4-5

> The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the "reset" command
>
> Asked Anthony Pejkovic how I would easily filter through and find the files in which he taught me this command.
>
>![lvl4-5.png](/banditimg/lvl4-5.png)

#### Level 5-6

> The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:
>    - human-readable
>    - 1033 bytes in size
>    - not executable