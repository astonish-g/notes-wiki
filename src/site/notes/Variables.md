---
{"dg-publish":true,"permalink":"/variables/","noteIcon":""}
---

##### Info:
In **Python** you can add **variables** in this way: 

```Python
variable_name = value
```

The `=` is the **assignment operator** . In this syntax, you assign a **value** to the `variable_name`. The value can be anything like a **number** , a **string** , etc.., that you assign to the variable. 

For example let's create a **variable** called ==name==.

```Python
name = ("Garo")
```

As you see above, we have put the name *Garo* as a **string** to the variable. Here's an example of using this variable:

```Python
character_name = ("Garo")
character_age = ("38")
print("He is a man named " + character_name + ", ")
print("and he is " + character_age + " years old.")
```

So the *program* above will give this output

```
He is a man named Garo,
and he is 38 years old.
```

As you can see on the example above, we are adding the *white space* to the **strings** as you need to place the spacing into it, if you want to create a correctly formatted text.

Also you can see that our variables in the examples are called:
- character_name
- character_age

Because in the **Python** coding language, when you use **multiple words**, it is a good practice to **seperate** the **words** with an **underscore** to improve the readability.

>[!Warning]
>You can't use some special characters like !,- in variable names. So, better stick to the words, numbers and underscore.
>
>Even if you can use numbers in variable name, you can NOT start with numbers for the variable names.
>
>Also note that, you can not use some special syntax words such as **if, for** in your variable names as they are reserved for syntaxes.


> [!note]
> Remember that a variable can hold various values at different times. So, you can change the value of the variable inside a program/script

##### Types of variables:
- ###### Global variable:
	The variables that are outside of the functions, are global variables and it will keep it's value throughout the code, unless you change it.

- ###### Local variables:
	Those are the variables that you create inside a function and they keep their value only inside this function.

- ###### An example:
	```Python
	x = 'awesone'
	
	def myfunc():
		x = 'fantastic'
		print('Python is ' + x)
	
	myfunc()
	
	print('Python is ' + x)
	```

	So in the example above, the value `awesome` belongs to a **global variable** whereas the value `fantastic` belongs to a **local variable**.
	
	The output will be like below:
	
	```
	Python is fantastic
	Python is awesome
	```

<br>

> [!Creating a global variable inside a function]
> If you want, you can create a **global variable inside a function**. To do so, you should use the `global` keyword.
> 
> ```Python
> def myfunc():
> 	global x
> 	x = "fantastic"
> 	
> myfunc()
> 
> print("Python is " + x)
> ```
> You can also use the `global` keyword to change a **variable** inside a function. 
> 
> ```Python
> x = 'awesome'
> 
> def myfunc():
> 	global x
> 	x = 'fantastic'
> 
> myfunc()
> 
> print("Python is " + x)
> ```


 


