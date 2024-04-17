---
{"dg-publish":true,"permalink":"/masking-services-to-install-tlp/","noteIcon":""}
---

##### General Info:
For TLP to install and work properly, you chould mask some of the services if you have a DE something like Gnome installed.

##### Power-profiles-daemon:
You should execute the command below to disable power-profiles-daemon:
```bash
systemctl mask power-profiles-daemon.service
```

##### Rfkill:
```bash
systemctl mask systemd-rfkill.service systemd-rfkill.socket
```