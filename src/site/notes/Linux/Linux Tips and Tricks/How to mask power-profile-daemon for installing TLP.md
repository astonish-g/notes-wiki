---
{"dg-publish":true,"permalink":"/linux/linux-tips-and-tricks/how-to-mask-power-profile-daemon-for-installing-tlp/","noteIcon":""}
---

TLP and Gnome profile daemon can go into conflict. To disable it, execute the below command in your terminal:

```bash
systemctl mask power-profiles-daemon.service
```

And I think that to unmask it, you should do something like this, but verify it first:

```bash
systemctl unmask power-profiles-daemon.service
```