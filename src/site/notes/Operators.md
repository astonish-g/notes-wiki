---
{"dg-publish":true,"permalink":"/operators/","noteIcon":""}
---

##### Info:
Operators are symbols used to perform operatios on values and the variables that hold those valuses. 

###### Basic operators:
 - ==Assignment Operator==
	 - For example when writing `name = 'Garo'` , in this case `name` is an **assignment operator**. If you type `color = 'green'` , then the `color` will be an assignment operator since we are assigning `green` as a value to it.
- ==Arithmetic Operator:==
	- **+** : Sum, plus
	- **-** : Minus
	- * : Multiplication
	- **/** : Divide
	- **//** : A division where it rounds the answer done.
		- For example `24 / 5` would give `4.8` as a result. But if you do `24 // 5` then it will round **down** the result to `4`. If you do it as `round(24 / 5)` then the result would be `5` because it **rounds it up**.
	- **%** : Gives the remainder. 
		- For example if you do `32 % 5` then it would give the result of `2` as after the division operation, `2` is what remains.
	- ** : The power of.
		- For example `7 ** 2` would give you the result of `49` as the power of 2 of 7 is 49 (7 x 7).
- ==Boolean Operators:==
	- == : Equal to. So if the result is not equal, then it will give `False` as output. If it is equal, than the output will be `True`
	- **!=** : NOT equal.
	- **>** : Greater than
	- **<** : Less than.
	- **>=** : Greater than or equal.
	- **<=** : Less than or equal.
	- **not** : It is what the name suggests.
		- For example let's say that we have a variable: 
			```Python
			x = True
			y = False
			z = True
			
			not x
			```
			And the output of the above program will be `False`.
	- **and** : This is an other boolean operator like not. But this adds two conditions. So let's take the example above.  
		```Python
		x and y
		```
		This evaluates the first value, and then evaluates the second one **ONLY** if the **first** value is **True**. So the output will be `False` because `y` is `False`.
	- **or** : So on the example above, it will check if x or y is true. So if one of them is true, it is enough to have a `True` output. 

###### Using operators with variables: 
```Python
meaning = 42
meaning += 1
```
will give you this output. 
```
43
```
As it means that it should do `42 + 1` and it will save that final value for the variable. So after this, if you do
```Python
meaning -= 1
```
Then the result will be:
```
42
```
As it will be doing `43-1` . We can use other operators like that too such as multiplication.
```Python
meaning *= 10
```
This means that it should multiply the value of `meaning` variable with `10` so the output will be:
```
420
```
And if i do:
```Python
name /= 7
```
Then the output will be:
```
60.0
```

###### Concatenate with operators:
You can use the operators to concetanate strings. For example

```Python
'Garo ' + 'Atmaca'
```
will output as:
```
Garo Atmaca
```