---
{"dg-publish":true,"permalink":"/how-to-set-the-undetected-filetypes-such-as-json-or-hyprlang/","noteIcon":""}
---

##### Info:
Let's say that you have set your tree-sitter..etc and sometimes it does not read detect the file type and it is not making correct highlighting. There are some ways you can do it.

> **This problem is caused when a file is saved without the extension name.**
##### This works always:
- While you are in normal mode, type the command below:
	- **:set filetype=hyprlang**

So the example above, sets the file type of the Hyprland configuration file to hyprlang and after doing this, it will do the correct syntax highlighting. You can do the same for **json** files without extensions as well, such as the **waybar config file:**
- **:set filetype=json**

And this will correct the syntax highlighting for the json file.

>[!warning]
>You have to do this each time you open that file.

##### Second workaround:
You can place a comment like this which tells nvim the file type:
```
# vim ft=hyprlang
```
After setting the example above, everytime that you launch your Hyprland configuration file, it will do the correct syntax highlighting.

> [!warning] 
> This did not work with the json file.