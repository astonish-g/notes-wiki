---
{"dg-publish":true,"permalink":"/numbers/","noteIcon":""}
---

##### Info:
You can use numbers inside Python and make all kind of mathematical operations with them, without an issue.

###### Types:
```Python
x = 1       # int
y = 2.8     # float
z = 1j      # complex
```

###### For example:
```Python
print (3 * 4.5)
```
An this will result in
```
13.5
```
You can also use parenthesis to specify the order of the operations like in real mathematics. For example:
```Python
print(3 * 4 + 2)
```
will result in 
```
14
```
as it will do the multiplication first since there are no paranthesis. And in the example below:
```Python
print(3 * (4 + 2) 
```
will result in
```
18
```
because it will take the sum first and then multiply with 3.

###### Handling large numbers:
When number is **large**, it'll become **difficult** to **read.** For example:

```Python
count = 10000000000
```

In this case, to make it easier to read, you can use **underscore** to **group the digits**. Here's an example:

```Python
count = 10_000_000_000
```

When storing or displaying these numbers, Python **ignores** the **underscore**. The underscore **works** both for **integers** and **floats**. 

###### Converting between number types:
For certain operations, you may need an **integer** or a **float**..etc numbers. You can change those types like below. You can use the same technic to convert between other data types as well such as string..etc.

```Python
x = 1     # int
y = 2.8   # float
z = 1j    # complex

# convert from int to float:
a = float(x)

# convert from float to int:
b = int(y)

# convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```

With the method above, you will see that the data types will be converted succesfully.

> [!Warning]
> You can **NOT** convert complex numbers into another number type.