---
{"dg-publish":true,"permalink":"/how-to-insert-at-the-end-of-the-line/","noteIcon":""}
---

##### Info
When I navigate with **arrow keys** or **h,j,k,l** to the **end of the line** and press **i** to **enter** the **insert mode**, it always inserts just before the last character of the line and I have to always press the right arrow key to start typing. Apparently it is not the best way.

##### What is the correct way?
- Go to the line that you want to add something in the normal mode.
- Pres ==A== *(capital A)* and this is the **append** command. So this will **start** the **insert** mode, at the **end of the line**, **no matter where your cursor is.**

##### What if you want to insert / append at the end of a file?
In this case, **in normal mode**,  you have to first press **G** *(capital G)* and **o** *(small letter o)*. 