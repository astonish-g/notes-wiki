---
{"dg-publish":true,"permalink":"/boolean/","noteIcon":""}
---

##### Info:
In programming, you often want to check if a condition is **true** or **not** and to perform some actions based on the result.

To represent **true** and **false**, **Python** provides you with the **boolean** data type. The boolean value has a **technical name** as ==bool==.

The boolean data type has **two values**:
- **True**
- **False**

> [!Note]
> Note that **True** and **False** always start with **capital letters**.

The following **example** defines two **boolean** **variables**:

```Python
is_active = True
is_admin = False
```

For example when you **compare** two numbers, **Python** returns the **result** as a **boolean value**. For example:

```Python
>>> 20 > 20
True
>>> 20 < 10
False
```

Also **comparing** two **strings** **results** in a **boolean** value:

```Python
>>> 'a' < 'b'
True
>>> 'a' > 'b'
False
```

##### The bool() function:
To find out if a value is **True** or **False**, you can use the **bool()** function. For example:

```Python
>>> bool('Hi')
True
>>> bool('')
False
>>> bool(100)
True
>>> bool(0)
False
```

When a **value** evaluates to **True**, it's ==truthy==. And if a **value** evaluates to **False**, it's ==falsy==.

> [!The following are falsy values in Python]
> - The number zero ( **0** )
> - An empty string **' '**
> - **False**
> - **None**
> - An empty list **[ ]**
> - An empty tuple **( )**
> - An empty dictionary **{ }**
> 
> All the other values that are NOT falsy are **truthy** values.

##### Most values are True
- Almost any **value** is evaluated to `True` if it has some sort of **content.** 
- Any **string** is `True`, **except** ==empty== strings.
- Any **number** is `True`, **except** `0`.
- Any **list, tuple, set** and **dictionary** are `True`, **except** ==empty== ones.

###### Examples:
The following will return `True` :

```Python
bool("abc")
bool(123)
bool(["apple", "cherry", "banana"])
```

##### Functions can return a value:
You can create functions that returns a Boolean value:

```Python
def myFunction() :
	return True

print(myFunction())
```

So the **function** example **above** will return `True`.


