---
{"dg-publish":true,"permalink":"/cat/","noteIcon":""}
---

##### Info:
The command `cat` let's you view the contents of a file without opening it. 

##### How to use?
You should type `cat` followed by the **name** of the **file** that you want to **view** the **contents**. For example:

```bash
cat garo.txt
Hello world
```

As you can see on the example above, our file called **garo.txt** had a content which is **Hello world**. By using the `cat` command, we were able to **view** it's **content** ==without== opening the file. 

###### View multiple files at once:

With this command, you can also view the contents of several files at once. **Here's an example:**

```bash
cat garo.txt
Hello world
```

```bash
cat info.txt
Do not run this app on MacOS!
```

```bash
cat garo.txt info.txt
Hello world
Do not run this app on MacOS!
```

###### Use this with redirection command:
This can be useful for the **redirection command** `>`. For example, this way, you can **save** the **output** of **several files** into a **single file**. For example:

```bash
cat garo.txt info.txt > final.txt
cat final.txt
Hello world
Do not run this app on MacOS!
```
