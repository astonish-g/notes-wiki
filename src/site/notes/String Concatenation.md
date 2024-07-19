---
{"dg-publish":true,"permalink":"/string-concatenation/","noteIcon":""}
---

##### Info
To concatenate, or combine, two strings you ckan use the `+` **operator**.

###### An example:
```Python
a = "Hello"
b = "World"
c = a + b
print(c)
```

So the output of the above code will be like this: 

```Python
HelloWorld
```

###### How to add space?
Actually you can do it in 2 modes. One of them would be adding a blank string between the variables. Here's an example:

```Python
a = "Hello"
b = "World"
c = a + " " + b
print(c)
```

Or, you can include the space in one of the strings. Here's how to do it:

```Python
a = "Hello"
b = " World"
c = a + b
print(c)
```

The output of both of them will be the same, as follows:

```
Hello World
```