---
{"dg-publish":true,"permalink":"/how-to-copy-a-list/","noteIcon":""}
---

##### Info:
When you want to copy a list, using a code like `new_list = my_list` will not work. They will both point to the same list. So to solve this, you should use **slice** instead.

##### How to do it?
You should point your new list to a slice of the previous list by omitting both the beginning and the end, so it will copy the whole list. Here's an example:

```Python
new_list = my_list[:]
```