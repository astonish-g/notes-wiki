---
{"dg-publish":true,"permalink":"/how-to-change-the-color-of-the-themes-with-variables/","noteIcon":""}
---

##### Info:
Sometimes when you are modifying some colours of a theme, it may be a little bit long to modify colours of each element one by one. Especially if there are some variables that are set.

##### Solution:
- Open the developper mode with `ctrl + shift + i`
- On the section where there are values, scroll down.
	- You will see things like `--inline-title-color`
	- Choose the element that interests you. ( You can search for items on the top where it writes filter. )
- Then in your CSS snippet, do as below:

```css
body {
	--inline-title-color: #8FBCBB !important;
	--link-color: #green !important;
	--link-color-hover: #D08770 !important;
	--list-indent: 2em !important;
}
```

This way you **will modify** the **variable** colors or values for a more genaralized and easy change.

As you see above, you can also change the values, such as the **value** for the **list-indent** on the example above.

> [!Tip]
> Save your CSS snippets with the name of the theme you are modifying, this way, when you change themes, you know which snippet to use, to keep your customizations.