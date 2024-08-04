---
{"dg-publish":true,"permalink":"/f-strings/","noteIcon":""}
---

##### Info:
As we know, in Python Variables, we can **NOT** combine **strings** and **numbers** like this. 

##### So what to do?
Apparently we can combine strings by **using** `f-strings`. Or you can use `format()` method. 

##### How to use the F-Strings:
F-Strings was introduced in **Python 3.6** and is now the **preferred way** of **formatting** strings.

To specify a string as an **f-string**, simply put an `f` in **front** of the **string literal**, and **add** **curly brackets** `{}` as **placeholders** for variables and other operations.

##### An example to see this:
```Python
age = 38
sentence = f"My name is Garo, I am {age}"
print(sentence)
```

The example above will give this output:

```
My name is Garo, I am 38
```

So as you can see, we used `f` **before** the **string** that we want to **print** where we **include** both a **string** and **integer**.
Then you see in the **curly brackets** the **integer** variable that we added in it.

The **curly brackets** on this code is a ==place holder==. A placeholder can contain **variables, operations, functions** and **modifiers** to format the value. 

##### An example:
```Python
price = 50
text = f"The price is {price} dollars"
print(text)
```
So above, the **double brackets** are serving as a **placeholder** for the `price`. 

##### Modifier inside a placeholder:
A *placeholder* can include a **modifier** to format the value. A modifier is **included** by adding a **colon** `:` followed by a legal formatting type, like `.2f` which means **fixed point number with 2 decimals**.

###### Here's an example:
```Python
price = 59
text = f"The price is {price:.2f} dollars"
print(text)
```

##### Python Code inside a Placeholder:
A place holder can contain **Python** code, like math operations. For example to **perform** a **math operation** in the placeholder, and return the result:

```Python
txt = f"The price is {20 * 59} dollars"
print(txt)
```

And the output will be:

```
The price is 1180 dollars
```


