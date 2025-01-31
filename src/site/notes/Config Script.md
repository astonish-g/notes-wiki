---
{"dg-publish":true,"permalink":"/config-script/","noteIcon":""}
---

### Check and compare the local .config folder:
You should use a *for loop* for a repetitive task about checking:
- If the **config** file **exists** in the `~/.config/` folder.
- If it exists, **create** a **backup folder** in `~/.config/backup` and **copy** the **old config** in it.
- if it does **NOT exist** then copy the config folder in `~/.config`

### How to do this?
We begin the script by setting our **variables** to **find** the correct **local directories** on our system.
#### Set your variables:
```bash
CONF="$(echo $HOME)"
RICE="$CONF/Documents/config"
DOWNLOAD=$(pwd)
```
So on the code above, variables:
- **CONF** finds the correct path for the **Home Directory**
- **RICE** states the local **.conf** directory.
- **DOWNLOAD** as the name suggests, finds the path where the script is downloaded.

###### Why don't I use the absollute path (~) for Home?
When I tried using `~/` for the **Home** directory in my bash script, it was **not working** somehow. I made it work by:
- Making a variable that checks the home directory with `echo` command.
- By using `$HOME` always as an **absolute path** which worked according to my testings.

#### Create a list from the items in the /dot-files/.config folder:
```bash
declare -a myApps=($DOWNLOAD/config/*)
```

The command above **creates a list** with the **names** of the **folders** inside the `/dot-files/.config/` folder. This way we have a kind of **dynamic script** which we won't have to update each time we put a new config folder to our dot files.

#### Create a loop with these list items:
```bash
for dir in "${myApps[@]}";
do
  if ! [ -d "$RICE/$dir" ]; then
    cp -rf $DOWNLOAD/config/$dir $RICE
  else
    mkdir $RICE/.config-backup &&
      mv $RICE/$dir $RICE/.config-backup/$dir &&
      cp -rf $DOWNLOAD/config/$dir $RICE
  fi
done
```
The script above tells these in the exact order:
- For every item in the .config directory list, *the list that we have created in the previous step* :
	- If the **item** does **NOT** exist in the **local** `~/.config` folder :
		- Copy the **downloaded** `/.config` folder item to the **local** `/.config` folder.
	- **Or** else, **if** it **exists**, then :
		- **Create** a folder called `/.config-backup` inside the `/.config` folder.
		- **Move** the **existing** config folder to the newly created `/.config-backup` folder.
		- Then **copy** the **downloaded** `/.config` folder into the local `/.config` folder.


##### But it does NOT work! Why?
Because each list item is saved with the full directory. For example:

`/home/username/Downloads/dot-files/config/fasfetch`

Because of this reason, using the **dir variable** is not working to specify the **copy destination.** 

###### How to fix this?
To fix this, we should **extract** the **name** of the **folder**. So we should only keep the part after the `/config/` in the directories listed with the **dir variable**.

We can do this by **creating** an other **variable** inside the **for loop**:
```bash
for dir in "${myApps[@]}";
do
  if ! [ -d "$RICE/$dir" ]; then
    cp -rf $DOWNLOAD/config/$dir $RICE
  else
    mkdir $RICE/.config-backup &&
    ITEM=${dir#*config/}
    mv $RICE/$ITEM $RICE/.config-backup/$ITEM &&
    cp -rf $DOWNLOAD/config/$ITEM $RICE
  fi
done
```

So on the code above: 

- We are **creating** a new **variable** called *ITEM*. 
- And we are telling it to **delete** everything before and including the `config/` in the directory name. 

This way we **obtain** only the **name** of the **folders** inside the the **downloaded config** folder.

> [!NOTE]
I still have an issue. It still is not copying the existing files to the folder.