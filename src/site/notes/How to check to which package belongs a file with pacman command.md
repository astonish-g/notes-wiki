---
{"dg-publish":true,"permalink":"/how-to-check-to-which-package-belongs-a-file-with-pacman-command/","noteIcon":""}
---

##### Info:
The other day, when I tried to update the system with `sudo pacman -Syu` it gave me several errors telling that some of the several files exists already in the file system and that the operation was failed.

##### How did I fix it? 
- First of all I searched to **which package it belonged** with the command `pacman -Qo /path/to/the/file
- This command outputs the name of the package the file belongs to.
- I deleted the file.
- Applied the update.
- Reinstalled the file.