---
{"dg-publish":true,"permalink":"/linux/hyprland/hyprland-installation-script/","noteIcon":""}
---

- [ ] Remember to install noto-fonts-emoji for Obsidian
- [ ] Remember to create the bluetooth udev rule
- [ ] Remember to create the udev rule for the Keychron and Nuphy keyboard

##### What should the script do?
The script should do these in this order:
- [ ]  It should **install** ==hyprland-git== with **yay**.
- [ ]  It should **install** ==xdg-desktop-portal-hyprland==. See [[Linux/Hyprland/How to use Gnome and Hyprland on the same user\|How to use Gnome and Hyprland on the same user]]
- [ ] It **should check** if you have the **necessary apps installed**:
	- [ ] alacritty
	- [ ] kitty
	- [ ] waybar *(Install the waybar-git version for [[Linux/Hyprland/waybar upower module\|waybar upower module]]*
	- [ ] wofi
	- [ ] ulauncher - using wofi instead
	- [ ] swaybg
	- [ ] feh
	- [ ] grim
	- [ ] slurp
	- [ ] nemo
	- [ ] nemo-fileroller
	- [ ] nwg-look (for theme changing on wayland)
	- [ ] swayidle - *Idle management daemon to handle idling sessions.*
	- [ ] swww - *to change wallpapers in x minutes*
	- [ ] catppuccinifier
- [ ] It should ask **one by one** if you **want** ==VSCode, Blender, Discord and BetterDiscord== installed.
- [ ] **Check** the **~/.config** folder for the ~/.config folders that **it will change**, such as ==alacritty, hypr, waybar==..etc.
- [ ] If it **finds any** then it should **create** a ==config.bak== folder in your **~/Documents** folder with all those folders **copied** in it.
- [ ]  Then it should **delete** those folders from the **~/.config** folder.
- [ ]  Then it should **copy** the folders to the **~/.config** directory from the ==dotfiles== folder. 
- [ ] Then it should **check** if you have **~/.local/share/fonts** folder and if you don't have it, it should **create** and **copy** the used ==fonts== to the **~/.local/share/fonts** directory. **If** you have it, then it should **just copy** the used fonts. 
- [ ] If you have selected to install **Discord** and **Better Discord** then it should **copy** the **BetterDiscord** .config folder as well.
- [ ] It should **create** a ==g-wallpapers== folder in **~/Pictures** folder and **copy** the **wallpapers** to that folder.
- [ ] It should **copy** ==Obsidian== and ==stylus-css-themes== folders to **~/Documents** folder.
- [ ] It should **check if** you **have** ==~/.themes== folder. **If** you **do** then it should **copy** the necessary **themes** from **/hypr-catppuccin-dotfiles/.themes** folder to your **~/.themes** folder. **If** you **do not**, then it should **copy** the **/hypr-catppuccin-dotfiles/.themes** folder to your **$HOME** folder.
- [ ] **If** you choose **to install** ==VSCode==, then it should **copy** the **.vscode-oss** folder to your **$HOME** folder and **/.config/code-oss** folder to your **~/.config** folder.
- [ ] **If possible** make it **copy/create** ==instrcutions== on **how to install** ==settings cycler== extension for **VSCode**.
- [ ] Make it **ask if** you **want** to **disable** ==bluetooth usb autosuspend==. **If** selected **yes** , then it should **find** the ==idVendor== and ==idProduct== and **create** the **correct udev rule**.
- [ ] Make it **install** ==oh-my-bash== and **copy** the **oh-my-bash** configuratiot to your **$Home** folder.
- [ ] **Set** the **GTK Theme** to **Catppuccin**.
- [ ] **Git clone** the ==Nordzy== icon theme. **Run** the **installation script** inside the folder. **Delete** the **downloaded** git-clone folder **after** installation. Finally **set** the **icon theme** from **terminal**. *(is it possible? yes it is possible! Check this: [[Linux/Hyprland/How to change icon theme from terminal\|How to change icon theme from terminal]] )* 
- [ ] Ask to ==restart== the **computer** and restart.