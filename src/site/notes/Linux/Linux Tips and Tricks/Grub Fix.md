---
{"dg-publish":true,"permalink":"/linux/linux-tips-and-tricks/grub-fix/","noteIcon":""}
---

> [!tip] Install arch-chroot-build
> Install **arch-chroot-build** package before doing this process. Then continue the process like below, and this way you can do it even without live usb if you have a second partition. 

**Fixing corrupted grub:**

- Log in from a liveuser usb, connect it to the internet and open the terminal.

- Execute these commands:

```bash
sudo su
```

- Then check your disk partition information with:

```bash
fdisk -l
```

- Then mount the boot partition and the Linux partition that you want to fix.

```bash
mount /dev/sda4 /mnt
mount /dev/sda1 /mnt/boot/efi
``` 

```bash
arch-chroot /mnt
```

> [!warning] 
> if your terminal says *bash: arch-chroot: command not found* , try `chroot /mnt` instead. 

```bash
grub-install --target=x86_64-efi --efi-directory=/boot/efi --bootloader-id=EndeavourOS
```

```bash
grub-mkconfig -o /boot/grub/grub.cfg
```

**How to update grub on Arch menu:**

On Arch linux, you don't have the update-grub command unless you install it from AUR. So to update grub, it is enough that you type this command in terminal:

```bash
grub-mkconfig -o /boot/grub/grub.cfg
```

And your grub config will be updated. update-grub commands runs the command above, so it does the same thing.

When you edit your grub, such as adding quiet splash..etc, you should always update the grub config later or else the changes will not work.