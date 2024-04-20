---
{"dg-publish":true,"permalink":"/obsidian/digital-garden/style-css-settings-not-applying-on-new-installation/","noteIcon":""}
---

I have realized that when I recreated the Digital Garden deploy repo, my site had lost the Catppuccin CSS styling that I had created and even though I had changed the **custom-style.css** file in the repo, still it looked unchanged.

##### The reason:
The reason was because when I reinstalled Obsidian, it was using the **default settings** for **Digital Garden** plug-in. 

##### The Fix:
- Go to **Obsidian settings**.
- Go to the **Digital Garden settings**.
- Go to **Appearance** section and click on **Manage appearance** button.
- On the window that opens, on the top section, click on the **Apply Style settings** button.

This will deploy your custom Obsidian CSS styles to the web-site. For some small things that it doesn't change, you do it with the **custom-styles.css** file that you have in your repository. 

But since you have already modified it, now it should apply all the modifications and your site should look nice again.