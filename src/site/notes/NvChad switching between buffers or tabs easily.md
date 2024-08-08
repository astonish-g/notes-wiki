---
{"dg-publish":true,"permalink":"/nv-chad-switching-between-buffers-or-tabs-easily/","noteIcon":""}
---

##### Info:
NvChad has some very useful keybindings. Here what I found useful to browse thru buffers and files:

##### How it works:
- **\<leader> ff :** Find files in the root directory with telescope.
- ==In Normal mode== **TAB** to switch between the open buffers/tabs.
- **\<leader> x :** To close the selected/opened buffer.

##### Multiple save:
In Neovim, when you type **:q** it closes the actual buffer. But if you have several buffers open, you can use **:qa** to close all of the buffers. So here, the a stands for all. You can do this to save all the files as well, or to close all the files without saving such as:
- **:qa!**
- **:wqa!**