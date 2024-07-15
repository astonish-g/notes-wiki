---
{"dg-publish":true,"permalink":"/how-to-open-the-file-tree/","noteIcon":""}
---

##### Info:
The **file-tree** (NvimTree) can be useful when you are trying to navigate between files in a project.

##### How to access it?
Inside the NVChad:
- Press **Ctrl** + **N** 

And you can close it with the same shortcut.

##### How to navigate between the buffer and the file tree?
You can use the general **VIM** keybindings with the key **CTRL**. So in this case:
- **Ctrl** + **h :** To move to the left. So if your file tree is on the left, the cursor will move to it.
- **Ctrl** + **l** : To move to the right. So if your buffer is on the right, then you can go to the buffer from the file tree by pressing this key combination.

While you are in the file tree with the cursor, you can open folders and files by pressing **enter** after **selecting** them with the **cursor**.

###### Some Shortcuts:
- ==R :== Refresh. To perform a reread of the files contained in the project.
- ==H :== Hide. To hide/display hidden files and folder.
- ==E :== Expand all. To expand the entire file tree starting from the root folder.
- ==W :== Collapse all. To close all open folders starting from the root folder.
- ==- :== Dir up. Allows you to go back up folders. This navigation also allows you to exit he root folder (workspace) to your home directory.
- ==s :== System. To open the file with the system application set by default for that file type.
- ==f :== Find. To open the interactive file search to which search filters can be applied.
- ==F :== To close the interactive search.
- ==Ctrl + k :== To display information about the file such as size, creation date, etc.
- ==g + ? :== To open the help with all the predefined shortcuts for quick reference.
- ==q :== To close the file explorer.

##### How to open the files from the file-tree?
- When you **select** the **file** and press ==enter== or ==o==, it **opens** the file in a **new buffer**.
- Press **Tab** to open the file in a **new buffer** while keeping the **cursor** on the **file-tree**.
- Press **Ctrl** + **t** to open the file in a **new tab** that can be managed separately from the other buffers present.
- Press **Ctrl** + **v** to open the file by splitting the buffer in vertical.
- Press **Ctrl** + **h** top opoen the file by splitting the buffer in horizontal.

##### File Management:
Continue typing from this link: https://docs.rockylinux.org/books/nvchad/nvchad_ui/nvimtree/

