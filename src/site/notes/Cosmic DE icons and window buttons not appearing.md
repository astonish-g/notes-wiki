---
{"dg-publish":true,"permalink":"/cosmic-de-icons-and-window-buttons-not-appearing/","noteIcon":""}
---

##### Info:
When I installed **Cosmic DE** on **Arch** Linux, I saw that the icons in file manager and the window icons on the app are not appearing, such as the window decorations. Apparently, the reason for this is the Vulkan drivers which were not installed properly on Arch or which I had to install manually. 

##### Solution:
To solve this, you need to use these following commands to install the necessary drivers:
- `sudo pacman -S --needed lib32-mesa vulkan-radeon`
- `sudo pacman -S --needed lib32-vulkan-radeon vulkan-icd-loader
- `sudo pacman -S --needed lib32-vulkan-icd-loader`

When I installed these packages in the following order above, when I was trying to install `lib32-vulkan-icd-loader` it told me that it was already installed. After installing all these packages, this **solved**, for me, the issues in the **Cosmic Desktop Environment**.