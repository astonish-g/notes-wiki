---
{"dg-publish":true,"permalink":"/slicing-strings/","noteIcon":""}
---

##### Info:
You can return a **range of characters** by using the **slice syntax**.

To use this, **specify** the **start** and the **end** index, **separated by a colon**, to return a part of the string.

###### Example:
The example below, will get the characters from the position 2 to position 5 *(position 5 is not included)*

```Python
b = "Hello, World!"
print(b[2:5])
```

And the code above will give the following output:

```
llo
```

> [!Note] 
> Note that the chosen end index is not included in the print. So when you choose a range to slice, it always includes the beginning but not the ending.

###### What if you want to slice from the start?
By **leaving out** the **start index**, the range **will start** at the **first character**.

```Python
b = "Hello, World!"
print([:5])
```

As you can see above, the beginning part of the index is not written, so this means that it starts from the beginning. You can do the same thing for the end of the string as well such as:

```Python
b = "Hello, World"
print([2:])
```

And in this case, the print will start from the third character (index 2) and will end at the end of the string.

You can also use **negative indexing** to **start** the **slice** from the **end of the line.** Here's an example:

```Python
b = "Think Different"
print(b[-5:-2])
```

And the output of the above code will be:

```
ere
```
