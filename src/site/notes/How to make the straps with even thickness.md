---
{"dg-publish":true,"permalink":"/how-to-make-the-straps-with-even-thickness/","noteIcon":""}
---

##### Info:
When you are using **curves** to make the straps of the shoes and then use a **taper object** to taper the general shape of the strap, then when you **convert** it to **mesh**, you will realize that you have **uneven thickness** and this will create a **problem** when you want to **bevel** it. 

##### Solution:
I kind of found an easy way to fix this:
- **Create** your **shape** with the **curves**.
- Once satisfied with it, **add** your **taper object** and modify the taper object's shape to the desires profile.
- **Convert** your **curve** to **mesh**.
- **Choose** the **outer faces** and **seperate** it from the rest by pressing **P**.
- **Delete** the rest of the converted **mesh**.
- On this stage you can modify the shape to make **micro adjustments**.
- **Add solidify** modifier and **enable** the **even thickness** option. 

This way you will be able to create an even thickness to your mesh that you have created with the curve.