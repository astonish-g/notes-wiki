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

###### Single Quotes and Double Quotes:
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

###### What if you don't want to escape the character with `\` but instead you want to include it in your string?
Well you can do it by inserting `r` before the first quote. Here's an example:
```Python
message = r'C:\python\bin'
```
In the example above, the character `\` will be used as it is. 

###### Triple Quotes:
You can also use **triple single quotes** or **triple double quotes** in your strings. They are used for **multiple line strings**.

Here is an example below:
```Python
s = ''' string can span
		multiple line '''
print(s)
```

The example above will output as:

```
string can span
multiple line
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

###### F-strings:
F-strings, let's you use the value of a variable, inside an other variable.  You do it by placing the letter `f` **before** the opening **quotation** mark and put the **brace** around the **variable name**.

For example:
```Python
name = 'Garo'
message = f'Hi {name}'
```

And the output will be:
```
Hi Garo
```

This feature was introduced with the Python version 3.6.

###### Slicing Stings:
**Slicing** allows you to get a substring from a string. For example:

```Python
car = 'Astonish'
print(str[0:5])
```
will slice the string and give you as an output the range between the index 0 and 5:
```
Aston
```
The `car[0:5]` returns a substring that includes the character from the **index 0** (included) to **5** ==(excluded)==.

The **syntax** for **slicing** is as follows:

```Python
string[start:end]
```

The substring always **includes** the character at the **start** and **excludes**  the string at the **end**.

While **slicing**, putting the **start** or the **end** is ==optional==. If you don't put the start, then it will default to **zero**. If you don't put the end, then it will default to the **string's length**.

###### How to modify the strings with slicing?
It is easier to explain it with an example.
```Python
string = 'Lamborghini'
string_new = 'W' + string[1:]
print(string.new)
```

So basically, **strings are immutable**. You can **NOT** modify a string. If you need to do it, you have to **create** a **new string**. 

If you check the example above, it is **NOT** modifying the original string. Instead, it is **creating** a **new string** called `string_new` . The new string is created with the **concatenation** of the letter **W** and the **original string without the first letter** by **slicing** it because we did not specify the **end** of the slice, so it takes the **full length** of the **string** after the **first letter**.

So the output will be like the following:
```
Wamborghini
```

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