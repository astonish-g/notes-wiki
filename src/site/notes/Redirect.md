---
{"dg-publish":true,"permalink":"/redirect/","noteIcon":""}
---

This command let's you **redirect** the **output** of any **command** **to any file**. The command is achieved by using the `>` symbol between the command and the output file name. For example:

```bash
echo "hello world" > newtext.txt
```
The example above will save the output of the command `echo "hello world` into a file called `newtext.txt` . But ==be careful:==
- if the file **does NOT** exist, this command will **create** it for you.
- If the file **does** exist, this comand will **overwrite** the contents of the file.

###### For example:
Let's say that a file called `newtext.txt` exists and it's **content** is *goodbye stranger*:
```bash
cat newtext.txt
goodbye stranger
```
And we direct the output of an other command to it:
```bash
echo "hello world" > newtext.txt
```
As a result, the *goodbye stranger* content will be deleted and replaced with the output of our `echo` command, so it will become *hello world* as seen below:
```bash
cat newtext.txt
hello world
```

###### How to append the output instead of overwriting?
To achieve this, instead of using a single `>` sign, you should use double `>>` sign. As a result, this will not overwrite the content, but instead, it will append it to the existing content. For example:

```bash
cat newtext.txt
goodbye stranger
echo "hello world" >> newtext.txt
cat newtext.txt
goodbye stranger
hello world
```