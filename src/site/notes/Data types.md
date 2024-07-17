---
{"dg-publish":true,"permalink":"/data-types/","noteIcon":""}
---

##### Info:
Variables can store data of different types. In **Python**, you have the following data types by default:
- ==Text Type:==
	- [[String\|String]] - for text
		- Strings are text.
		- They are written in `""` double coma.
- ==Number Types:==
	- [[Integer\|Integer]] - for **NON** decimal numbers
		- These are numbers. They can **NOT** include **decimals**. For example: `3`
	- [[Floating\|Floating]] - for decimal numbers
		- These are numbers too **BUT** they **CAN** include **decimals**. For example: `3.14`
	- `Complex`
- ==Mapping Type:==
	- `Dict`
- ==Set Types:==
	- `set`
	- `frozenset`
-  ==Boolean Type:==
	- `bool` - read [[Boolean\|Boolean]] for more info.
- ==Binary Types:==
	- `bytes`
	- `bytearray`
	- `memoryview`
- ==None Type:==
	- `NoneType`

##### Getting the Data Type:
You can get the data type of any object by using the`type()` function:

```Python
x = 5
print(type(x))
```

This should give an output that gives information about the data type of the variable x:

```
<class 'int'>
```

So as you see above, the **output** tells us that the **data type** of the **x** variable's **value** is an **integer**.

##### Setting the Data Type:
In Python, the data type is set when you assing a value to a variable:

###### Examples:
- `x = "Hello World"` = ==str==
- `x = 20` = ==int==
- `x = 20.5` = ==float==
- `x = 1j` = ==complex==
- `x = ["apple", "banana", "cherry"]` = ==list==
- `x = ("apple", "banana", "cherry")` = ==tuple==
- `x = range(6)` = ==range==
- `x = {"name" : "John", "age" : 36}` = ==dict==
- `x = {"apple", "banana", "cherry"}` = ==set==
- `x = frozenset({"apple", "banana", "cherry"})` = ==set==
- `x = True` = ==bool==
- `x = b"Hello"` = ==bytes==
- `x = bytearray(5)`  = ==bytearray==
- `x = memoryview(bytes(5))` = ==memoryview==
- `x = None` = ==None==

###### You can also set a specific data type:
- `x = str("Hello World!")` = ==str==
- `x = int(20)` = ==int==
- `x = float(20.5)` = ==float==
- `x = complex(1j)` = ==complex==
- `x = list(("apple", "banana", "cherry"))` = ==list==
- `x = tuple(("apple", "banana", "cherry"))` = ==tuple==
- `x = range(6)` = ==range==
- `x = dict("name" : "John", "age" : 36)` = ==dict==
- `x = set(("apple", "banana", "cherry"))` = ==set==
- `x = frozenset(("apple", "banana", "cherry"))` = ==frozenset==
- `x = bool(5)` = ==bool==
- `x = bytes(5)` = ==bytes==
- `x = bytearray(5)`  = ==bytearray==
- `x = memoryview(bytes(5))` = ==memoryview==

> [!Note]
> Note how the syntax changes from brackets..etc to paranthesis when you set a specific type.
