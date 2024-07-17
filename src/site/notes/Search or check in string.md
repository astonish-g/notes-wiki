---
{"dg-publish":true,"permalink":"/search-or-check-in-string/","noteIcon":""}
---

##### Info:
In Python, you can use the **keyword** `in` to check if a character or a phrase is present in a string.

###### Example:
```Python
txt = "Moscow Mule is the best coctail."
print("best" in txt)
```

The code above will give a `bool` output. If it is present, it will output as `True`.

You can use it in an `if` statement. The statement below will **print** ==ONLY if== free is present.

```Python
txt = "Moscow Mule is the best coctail."
if "free" in txt:
	print("Yes, 'free' is present.")
```

So the example above will give this output:

```
Yes, 'free' is present.
```

##### How about checking if it is NOT present?
Then in this case, you should use the **keyword** `not in`. Here's an example:

```Python
coctail = "Moscow Mule is the best coctail."
print*("Miami" not in coctail)
```

Obviously the example above will give `True` as a **value** since it is **NOT present** in the variable.

You can put it in an `if statement` as well like we did before. Here it is how:

```Python
coctail = "Moscow Mule is the best coctail in the world."
if "Miami" not in coctail:
	print('Miami" has nothing to do with this coctail.')
```
