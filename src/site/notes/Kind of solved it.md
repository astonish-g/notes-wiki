---
{"dg-publish":true,"permalink":"/kind-of-solved-it/","noteIcon":""}
---

So kind of I am understanding how to do it and I made some progress on the rivets on how to do it. 

##### What I did?
- **Selected** an **edge loop** which could serve as a path for my rivets, and **dupplicated** it.
- Then I **separated** it by **pressing** the **P** key.
- **Selected** the newly **seperated edge loop** and **right clicked** on it and:
	- **Convert to > Curve**
- **Created** a **rivet** from a cylinder. 
- **Selected** the **curve** and **set** the **origin** of the **curve** to it's **center**.
- Then with **Shift + S**, with the **curve selected**, I clicked on **cursor to selected** to bring the **3D cursor** to the origin of the curve.
- **Select** the rivet, and with **Shift + S**, choose **Origin to Geometry**. 
- Then with the **rivet** always **slected**, again with **Shift + S**, I clicked on **Selection to cursor**.

##### Making the array:
- Selected the **rivet** and added an **array modifier**.
- On the array modifier, I set a **Factor X** to **1.500** to set a distance between the rivets (change it as you like) and **increased** the **number** of **count** to **44** to cover the full distance of the curve. Again, here, you can set a number that fits your case.
- Finally, **add** a **curve modifier** and **choose** the created curve as **Curve Object**.

>[!Warning] 
>Unfortunately, the rivets are not really rotating in all the axis to follow the normals. so I may need to modify the curve with it, rotating each CV of the curve, to make the normals look the correct way, or else, I still have to find the correct way.