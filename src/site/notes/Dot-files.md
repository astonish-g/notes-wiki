---
{"dg-publish":true,"permalink":"/dot-files/","noteIcon":""}
---

##### Info:
A brief **to do list** of the things that I still have to do to finish the **dot-files.**

##### Things to do:
- [x] Add **touch to tap** to the i3 installer script.
	- Created the script, now need to add it to the general installation script.
- [x] Import **nemo** file manager settings.
	- You should do these with `dnf write` commands. For example, to set the icon size in the nemo, you should type in your script `dconf write /org/nemo/icon-view/default-zoom-level "'larger'"`
- [x] Import lxappearance settings. 
	- You should back-up the GTK-3 folder from the .config folder to import the settings of lxapearance. 
- [x] Find the right font size for **alacritty** terminal inside the config file and replace the repo files with it. 
	- The one used in my i3 installation is **alacritty-i3**. And font size 16 is good. 15 is nice as well but with 16 the padding looks better.
- [x] Include an **Obsidian** config file without giving the github token.
- [x] Solve the VSConfig folders not working under Fedora.
	- I solved it by installing **VSCodium** and replacing and renaming the **Code - OSS** config folders both in **Home** and **~./config** directory with the correct names that the **VSCodium** uses for it's configs. The settings didn't work with **Vanilla VSCode**, so install **VSCodium** on **Fedora**.
- [ ] Include g-scripts.
- [x] Make a **GitHub** installer with **variables** instead of using my username and e-mail. Make the variables take the user name and the e-mail from the user inputs in the script.
- [x] **Copy** multiple files with one command such as `cp -r ~/Downloads/i3-new-dotfiles/.config/* ~/.config/` instead of doing these one by one in the command.
	- [ ] ==Need to test this!==
- [x] Add an **Obsidian install** script or add it to the i3-rice-installation script.
- [ ] Import Firefox settings from terminal if it is possible.
- [ ] Check if you can include the settings-cycler in VSCodium from terminal. 
- [ ] Set **xrandr** to **auto** mode.
	- Something like xrandr --output eDP-1 --auto

##### Nemo Settings to copy:
- [x] Icon size - Zoom level
	- dconf write /org/nemo/icon-view/default-zoom-level "'larger'"
- [x] Hide menu bar
	- dconf write /org/nemo/window-state/start-with-menu-bar false
- [x] Hide Status bar
	- dconf write /org/nemo/window-state/start-with-status-bar false
- [x] Thumbnail preview image size in mb
	- gsettings set org.nemo.preferences thumbnail-limit 1073741824
	- ==it is giving errors==
- [x] Inherit view type (icon, compact, list) from parent to children
	- dconf write /org/nemo/preferences/inherit-folder-viewer true