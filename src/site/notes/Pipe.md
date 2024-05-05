---
{"dg-publish":true,"permalink":"/pipe/","noteIcon":""}
---

##### Info:
This command let's you use the **output** of a comand as the **input** of a command. It is done by using the symbol `|` **between** the commands. You can use **several pipes** at the same time.

##### How to use?
As explained above, you have to place `|` between the commands. For example:
```bash
ls A-folder/
1.txt  1a.txt  2.txt  3.txt  aaa.txt
```
Now let's use the output of the command above as the input of an other command:
```bash
ls A-folder/ | less
```
This will output as:
```bash
1.txt
1a.txt
2.txt
3.txt
aaa.txt
(END)
```

This is called **piping in a command**.  So if you hear or read it somewhere, this is exactly what it means.

##### How does it work?
So if we look at the example above. When we wrote this command, it first **redirected** the **output** of the `ls A-folder/` command to a *temporary file* such as this:
```bash
ls A-folder/ > temporaryfile.txt
```
Then when we view the contents of the temporary file, we will see that it is the **output** of the `ls` command:
```bash
cat temporaryfile.txt
1.txt
1a.txt
2.txt
3.txt
aaa.txt
```
And then when we give the **temporary output** to the command `less`, we achieve the result that piping has given us:
```bash
less temporaryfile.txt
```
```bash
1.txt
1a.txt
2.txt
3.txt
aaa.txt
(END)
```

##### Use several pipes:
As explained above, you can use several pipe commands together. For example:
```bash
ls A-folder/ | tail -3 | less
```
Which will result in an output like this.
```bash
2.txt
3.txt
aaa.txt
```
Because the `tail` command is used to view the last lines of a content in a file. For more info, check [[Tail\|Tail]] command.
