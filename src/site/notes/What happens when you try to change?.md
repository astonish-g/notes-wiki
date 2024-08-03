---
{"dg-publish":true,"permalink":"/what-happens-when-you-try-to-change/","noteIcon":""}
---

##### Info:
In the general info page, we have mentioned that you can not change the values in tuple.
If you try to change like in the example below:

```python
dimensions = (200, 50)
dimensions[0] = 250
```

Python will give you the following error:

```python
TypeError: 'tuple' object does not support item assignment
```