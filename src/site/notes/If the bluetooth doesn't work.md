---
{"dg-publish":true,"permalink":"/if-the-bluetooth-doesn-t-work/","noteIcon":""}
---

##### Info:
Today for a reason, my bluetooth stopped working. When I ran `bluetoothctl` it was still trying to connect to the bluetooth and when I tried starting the scan, it gave me this output:

`Failed to start discovery: org.bluez.Error.NotReady`

But when I did `systemctl status bluetooth` command, it was still showing working and running.

##### Solution:
Apparently it was the `rfkill` that was blocking it. So I did it this way to fix it:
- On terminal execute the command `rfkill list`
- Look at the output. Check to see if `soft block` or `hard block` is flagged as `yes` 
- If any of them is flagged as yes, then run the command `rfkill unblock all`

This should fix your issues if for some reason rfkill block was on again.