---
{"dg-publish":true,"permalink":"/how-to-remove-an-edge-loop-and-redistribute-the-remaining-ones-equally/","noteIcon":""}
---

##### Problem:
Sometimes you may want to decrease the number of the edge loops but you making it manually can be a tedious and less precise task. To be able to do it nicely, we can use the **Edge flow** plug-in.

##### Needed plug-in:
- Edge Flow

##### How to do it?
- Remove the unwanted edge loops.
- Select all the edge loops that remains between two edge loops that you want to redistribute.
- With the edge loops that you want to redistribute selected:
	- **Right click** and go to **Set Flow** submenu and click on **Set Flow**

After doing the steps above, your edge loops should be redistributed nicely.

<br>

>[!Warning] 
>Remember to keep two edge loops unselected. Those two edge loops will be the starting and end point of the redistribution area. If you select them as well, it will change the general geometry/edges of the surface.