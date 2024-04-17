---
{"dg-publish":true,"permalink":"/how-to-prevent-computer-going-to-sleep-or-turn-display-off/","noteIcon":""}
---

##### How to prevent computer to go to sleep to blank screen?
- You should open your **terminal**
- **Type** in the **terminal** window: 
	
	`xset s off`

The command above will turn off the default setting for turning the screen to blank like a screen saver after 10 minutes of inactivity. It is set to 600 seconds by default.

##### How to prevent computer display to turn off after inactivity?
- Again open your **terminal**.
- **Type** in the **terminal** window:
	
	`xset -dpms`

This command will disable the **dpms** which means *Display Power Manager Settings* and it will not turn off your monitor when you have like 10 minutes of inactivity such as watching a movie on Youtube..etc.

> [!Warning]
> Note that these settings that you change, will reset on each reboot. To make these settings permenant, you may need to add a script to your i3 WM config file which starts with the computer.

##### How to check current settings for these?
To check the current screen saver..etc settings on your computer, you should try the command:
	
	`xset q`

This will list all the current settings that you are using at the moment.

