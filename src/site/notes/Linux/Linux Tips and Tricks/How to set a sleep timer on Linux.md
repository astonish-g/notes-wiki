---
{"dg-publish":true,"permalink":"/linux/linux-tips-and-tricks/how-to-set-a-sleep-timer-on-linux/","noteIcon":""}
---

You can set a **sleep timer** on Linux like on televisions. It is very easy and you don't have to install anything to do so.

##### How to do it?
- Open your **terminal** window.
- Type the command: `sudo shutdown -P +60` and press **enter**.

This command above will schedule a shut down in **60 minutes** and when the time finishes, it will shut down the computer. It is as easy as this.

##### How to cancel a scheduled shutdown?
- You just need to type `sudo shutdown -c` and this will cancel the pending shutdowns. 

##### Commands Explained:
These informations were extracted from the `shutdown --help` command.
- `shutdown -P` = Power off the machine. P is in capital.
- `shutdown -r` = Reboot the machine.
- `shutdown -h` = Equivalant to `--poweroff`, overriden by `--halt`
- `shutdown -c` = Cancel a pending shutdown.
- `shutdown --show` = Show pending shutdown. 