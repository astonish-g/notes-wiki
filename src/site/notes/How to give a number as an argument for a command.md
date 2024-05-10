---
{"dg-publish":true,"permalink":"/how-to-give-a-number-as-an-argument-for-a-command/","noteIcon":""}
---

##### Problem: 
I have a script where it turns dpms off, screen sleep off and then adds a shutdown for the desired minutes, like a sleep timer. It works very well but it works with a default number. I would like to use that script that it asks me for a time or I add it as an argument to the script and that it changes the sleep timer to that desired minute.

##### Solution:
You can achieve this by adding a simple variable which will be the command argument. Let's make a script called **gotosleep.sh** and let's put this inside the script:

```bash
#!/bin/bash

# Display Power Management Signaling features off
xset -dpms

# Sets the screensaver off
xset s off

# Set timer limit to the argument
sudo shutdown -P $1
```

The script above will turn all the power management features off and will use as a time limit the first argument that user inputs with the command.

##### Command explained:
- `xset -dpms`
	
	In X server **dpms** means **Display Power Management Signaling**. And the command above **turns off** all the dpms features so this way your **display** do **not go** in **standby** mode.

<br>

- `xset s off`
	
	This command controls the screen-saver settings. So the command above will **turn off** the **screensaver** so while you are watching a video..etc during the sleep timer period, the monitor will not launch the screen saver.

<br>

- `sudo shutdown -P $1`
	
	This sets the timer limit for the shutdown process. By adding `$1` to the end of the command, we are telling to the **command** to **use** the **first argument** that we add to our bash script while **running** in **terminal** to be **used**.

##### Execution examples:
After placing this script to our path directory and let's **rename** it from *gotosleep.sh* to *gotosleep* so that we do **not need** to type **.sh** every time we want to run it, we can run it as:

- `gotosleep 20` 
	
	This will **set** the **shutdown timer** to **20 minutes**. 

On the other hand:

- `gotosleep 50`
	
	will the **set** the **shutdown timer** to **50 minutes**.