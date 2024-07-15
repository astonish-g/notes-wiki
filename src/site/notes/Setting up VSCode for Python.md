---
{"dg-publish":true,"permalink":"/setting-up-vs-code-for-python/","noteIcon":""}
---

##### Info:
By default, VSCode, does not come with the **Python** extensions. So, after you install **Pythong** on your computer, go to the **Extensions** tab of your VSCode and:
- Install Python extension from Microsoft. [[How to install\|How to install]]
- Press CTRL+Shift+P to open the **command window** and:
	- Type **Python Select Interpreter**.
	- Press **enter** on the selection.
	- Choose the recommended Python edition from that menu. 
- Also with Ctrl+\` open a new terminal (or from the top menu)
	- Type `python3` in terminal since you are in **Linux**. If you are on **Windows** then you should type `py3`. 
	- You can **hide** the terminal with Ctrl+\`

##### How to run your python scripts in VSCode for test?
- By **right clicking** to the name of your file on the file explorer and selecting **"Run Python file in Terminal**.
- By clicking on the **play button** that you have on your **tab bar**.
- Or by navigating to your file from terminal inside the VSCode and using the command: `python3 name_of_the_file.py`

##### Set the format on save and format on type:
- In VSCode, press Ctrl + , to open the settings.
- Type **format on save**.
- Put a **check** on it to **enable** it.
- Then search for **format on type**.
- **Enable** it as well.