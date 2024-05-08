---
{"dg-publish":true,"permalink":"/subdivision-modifier-on-cage-option/","noteIcon":""}
---

##### Problem:
When you use subdivision modifier, and when it is **on** and you go into **edit mode**, you see that your model goes **back** to the *un-subdivided* state in a *phantom* view but you may **prefer** to have your **edges** on the subdivided forms.

##### Solution:
- Add **subdivision modifier** to your modifiers.
- In the **modifier panel**, next to the modifier's **title**, so in this case, next to the **subdivision**, you have a **triangle shaped icon**. It is called **On Cage**. Click on it to **enable** it.
- Now you wil see your **edges follow the subdivided shape**.

With this method, you may have a general idea of how your topology may look. Obviously, it does not show you the subdivided face edges and it does not let you modify them unless you apply the modifier but still you have an idea. 

Actually, if you want to see how the subdivided edges will look, you can do it by:

- Going to the **Viewport Overlays** options on **top right** of your viewport.
- And then by **activating** the **wireframe** option.
- In your **Subdivision** modifier options, you should **disable/uncheck** the **optimal display** option.

**Now** you will be **able to see the edges of your surfaces** once the **subdivision** modifier will be **applied**. But you should **note** that this solution **only works in object mod**.