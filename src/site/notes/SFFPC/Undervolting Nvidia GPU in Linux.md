---
{"dg-publish":true,"permalink":"/sffpc/undervolting-nvidia-gpu-in-linux/","noteIcon":""}
---

>[!useful link] 
>[Nvidia Undervolting](https://linustechtips.com/topic/1259546-how-to-undervolt-nvidia-gpus-in-linux/)
>
>On the link above, you can see some useful information about undervolting Nvidia GPU on Linux. 
>
>In case the link gets deleted, here is the [[SFFPC/copy paste link\|copy paste link]] about Nvidia Undervolting till I type about it. 

##### Other useful links:
- [Nvidia Undervolting Github Comment 1](https://github.com/NVIDIA/open-gpu-kernel-modules/discussions/236)
- [Arch Wiki Nvidia Settings](https://wiki.archlinux.org/title/NVIDIA/Tips_and_tricks) - Check the part about **Overclocking and cooling**
- [Linux Mint Forums](https://forums.developer.nvidia.com/t/undervolting-can-damage-video-card/214471)
- [Post from Nvidia Foruma](https://forums.developer.nvidia.com/t/undervolt-powerlimit-4090-fe-on-redhat-linux/269726)
- [Reddit Post](https://www.reddit.com/r/linux_gaming/comments/15n4gmr/linux_undervolting/) - Check the post of **0xd00d**
- [Very interesting article on Medium](https://betterprogramming.pub/limiting-your-gpu-power-consumption-might-save-you-some-money-50084b305845) - Nvidia undervolting explained in a simple way.


>[!Tip] Check PowerMizer
>Seems like this is an app that helps to control the undervolting with UI.

> `nvidia-smi -pl 200` seems like is a command that sets the power limit to 200 watt for example.