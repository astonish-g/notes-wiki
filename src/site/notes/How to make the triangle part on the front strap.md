---
{"dg-publish":true,"permalink":"/how-to-make-the-triangle-part-on-the-front-strap/","noteIcon":""}
---

##### Info:
I had some issues while trying to do the triangle part on the front strap where there is the Prada logo. After making some trial and error, here's the way that I found it to be the *easiest* to do. The **topology** should still **be fixed**.

##### How to do it? 
- **Dupplicate** the **front strap** mesh.
- **Apply** the **subdivision** and **solidify** modifiers
	- For the **subdivision** modifier, **apply** it with **level 1** to make working on it easier.
- **Select** the **faces** in a kind of **rectangle shape** where you will be **creating** your **triangle**.
- With some **edge loops** on the **sides/edges** you can **modify** even more the **size** of the **rectangle** border. **Delete** the **excess faces** that are **outside** of the edge loops that you have added.
- You can **simplify** the geometry even more by deleting some **"unnecessary"** edge loops. 
- **Draw** the **triangle** and delete the **faces** in **excess**.
- **Extrude** the face to give it some **thickness**.
- **Bevel** the **edges** to give that **circular** triangle shape.

This should help to create that form. But the ==topology is not quads and clean, so you may try to fix it. ==