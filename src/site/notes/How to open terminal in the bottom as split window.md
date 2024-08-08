---
{"dg-publish":true,"permalink":"/how-to-open-terminal-in-the-bottom-as-split-window/","noteIcon":""}
---

##### Info:
In the default configuration of LazyVim, it does not open the terminal at the bottom like NVChad. But it is an easy fix.

##### How to do it?
1. In LazyVim, go to the **Extras** panel to control the extra plug-ins. You do this by **typing** in **normal mode** ==:LazyExtras== .
2. Then scrol down to till you find the **edgy** plug-in. You find it as ==ui.edgy==.
3. **Enable** it by pressing ==x==.
4. **Restart** LazyVim.
5. Then, you can toggle the terminal with ==Ctrl + /== shortcut.

> [!Note] 
> If you want the terminal to open in the directory of the file, you should first go to the directory of the file from terminal and then open it with the nvim command. Or else, it will open in the directory that you were in when launching the LazyVim app.

##### Switching between terminal and buffer:
If you want to keep the terminal open and swtich back and forth with the editor, you can use:
- **CTRL + J :** To go to the bottom split, in this case the terminal.
- **CTRL + K :** To go to the top split, in this case the editor.