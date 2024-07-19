---
{"dg-publish":true,"permalink":"/general-info/","noteIcon":""}
---

##### Info:
Lists are used to store multiple items in a single variable. 

> [!Data Types to store collections of Data]
> 4 built-in data types in Python used to store collections of data :
> - List
> - Truple
> - Set
> - Dictionary

**Lists** are **created** with **square brackets**.

##### Example:
```Python
this_list = ["apple", "banana", "cherry"]
print(this_list)
```

##### List Items:
- List items are:
	- ordered
	- changeable
	- allow dupplicate values

List items are indexed. The first item has **index** ==[0]== , the second item has **index** ==[1]== ..etc.

##### List items are ordered:
This means that the items have adefined order, and the order will not change.

If you add new items to a list, the new items will be placed at the end of the list.

##### List items are changeable:
The list is changeable, meaning that we can change, add and remove items in a list after it has been created.

##### Allow dupplicates:
Since lists are **indexed**, lists **can have** items with the **same value**. Here's an example below:

```Python
this_list = ["apple", "banana", "cherry", "apple", "cherry"]
print(this_list)
```

##### List Length:
To determine how many items a list has, use the `len()` function.  Here's an example:

```Python
thislist = ["apple", "banana", "cherry"]
print(len(thislist))
```

And the code above will give this output below:

```
3
```

So it counts the item numbers?

##### Data Types:
A List can contain items of any data type and you can also put them together, so it can contain different data types as well. Here's an example:

```Python
list1 = ["abc", 34, True, 40, "male"]
```

##### type()
From Python's perspective, lists are **defined** as **objects** with the data type **'list'** :

```
<class 'list'>
```

##### list() Constructor:
It is also possible to use the `list()` constructor when creating a new list.

Here' s an example:
```Python
thislist = list(("apple", "banana", "cherry")) # note the double round-brackets  
print(thislist)
```

> [!Note that with this technic, double round-brackets are used.]
> 

