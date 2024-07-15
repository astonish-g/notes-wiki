---
{"dg-publish":true,"permalink":"/pv/","noteIcon":""}
---

##### Info:
Monitor the progress of data through a pipe. So for example when you are making a copy or something, if you pipe the copy operation with the pv command it should appear a progress bar.

>[!warning] 
>This is not included in the vanilla Fedora installation, so if you include this into an installation, it may not work.

##### Useage:
It should work as something like this:
```bash
cp -r ~/Documents/Obsidian ~/Documents/Personal-notes/ | pv
```