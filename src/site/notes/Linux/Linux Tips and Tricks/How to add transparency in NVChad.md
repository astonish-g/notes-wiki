---
{"dg-publish":true,"permalink":"/linux/linux-tips-and-tricks/how-to-add-transparency-in-nv-chad/","noteIcon":""}
---

##### Tags

#nvchad

##### Content

> Browse to the file:
> 
> **~/.config/nvim/lua/custom/chadrc.lua**
> 
> open it with neovim and
> 
> **transparency = true,**
> 
> So the final output should be something like:
> 
> local M = {}
> M.ui = {
> 	{theme = 'catppuccin'};
> 	transparency = true,
> }
> 
> return M

