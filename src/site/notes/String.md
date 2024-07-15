---
{"dg-publish":true,"permalink":"/string/","noteIcon":""}
---

##### Info:
**String** is a data type in Python that includes **plain text**. You can include numbers too, but you can **NOT** use numbers as a string in mathematical operations.

###### Example 1:
```Python
print("Astonish Academy")
```
This will result in this:
```
Astonish Academy
```

###### Example 2:
What if you want to create a new line inside the string? You can do it by adding `\n` between the words like in the example below:

```Python
print("Astonish\nAcademy")
```
And the result will be like this:
```
Astonish
Academy
```

###### Quotation marks:
You can write **strings** with both **single** or **double** cotation marks. Here's an example:
```Python
print("Astonish Academy")
```
and
```Python
print('Astonish Academy')
```
will both result in this outpui:
```
Astonish Academy
```
This can be useful if you have to use `"` inside your string, this way it will **NOT** end the the string. For example:
```Python
print('Astonish "Academy"')
```
and this will result in
```
Astonish "Academy"
```
Or else if you want to use double quotation mark inside a double quoation mark string, you can use `\` because it has `escape character` value. For example:
```Python
print("Astonish\"Academy")
```
will output as
```
Astonish"Academy
```

###### String Variables:
You can also create string variables too. For example:
```Python
phrase = "Giraffe Academy"
print(phrase)
```
And this will output as:
```
Giraffe Academy
```

###### Concatenation:
This means taking a string and **appending** an **other string** onto it.

```Python
phrase = "Giraffe Academy"
print(phrase + " is cool.")
```
which will result as:
```
Giraffe Academy is cool.
```
Note the white space left in the beginning of the `" is cool."` string to add a space after the word `Academy`.

###### Functions Example 1:
You can use functions to **modify** your **strings** or to get **information** about our **strings**.

Here's an example:
```Python
phrase = "Giraffe Academy"
print(phrase.lower())
```
and this will output as:
```
giraffe academy
```
As you can see. It took the string and converted it all to lowercase letter.

###### Functions Example 2:
Now let's convert them all to upper case.
```Python
phrase = "Giraffe Academy"
print(phrase.upper())
```
and here's the output:
```
GIRAFFE ACADEMY
```

###### Functions Example 3:
You can also check if a string is entirely upper case. This will give you a **True** or **False** result. Here's an example:
```Python
phrase = "Giraffe Academy"
print(phrase.isupper())
```
and the output is:
```
False
```

###### Functions Example 4:
You can also use the functions in **combination** to **each other**. For example: 
```Python
phrase = "Giraffe Academy"
print(phrase.upper().isupper())
```
So the example above will first run the `upper` function, converting it all to the upper case and then will check with the `isupper` function to see if all the letters are upper case. And this is the output:
```
True
```

###### Function Example 5:
We can also figure out the **length** of our **string**. For example:
```Python
phrase = "Giraffe Academy"
print(len(phrase))
```
And the example above will count the number of characters that are inside the string and give the result as:
```
15
```

###### Function Example 6:
We can also **grab** an **individual character** from the **string**. For example:
```Python
phrase = "Giraffe Academy"
print(phrase[0])
```
Using the `[]` (open and close square bracket), we can specify the [[index\|index]] of the **character** that we want to grab. The example above will result in:
```
G
```

###### Function Example 7:
An other interesting function is **index**. This will tell use where a specific character is located in our string.
```Python
phrase = "Giraffe Academy"
print(phrase.index("G")
```
And the example above will return as the index of the character `G` and since it is the first letter in our string, the result should be:
```
0
```
The function above shows us the **first time** that the character appears in our string. You can also put words into it if you prefer:
```Python
phrase = "Giraffe Academy"
print(phrase.index(Acad))
```
and this will result in:
```
8
```

###### Function Example 8:
You can also replace characters or words with this function. For example:
```Python
phrase = "Giraffe Academy"
print(phrase.replace("Giraffe", "Garo"))
```
Note that here we have to put 2 arguments. This will result in:
```
Garo Academy
```