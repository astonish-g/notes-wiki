---
{"dg-publish":true,"permalink":"/solution/","noteIcon":""}
---

When I reinstalled linux on the computer and published notes, I had a problem that my notes would not deploy to the Vercel page. 

##### The reason:
I had **deleted** the **repository** from which **Digital Garden** was **deploying** the notes to the **Vercel** app and I had **created a new one**. But the **token** that I had created for the Digital Garden was **searching** for the **old repository** that was **deleted** and was not considering the newly created Digital Garden repository. 

##### The solution:
- Go to **Github** page and open the **settings** page.
- From the sections, choose the **Developper Options** section.
- From the page that opens, choose the **Fine Grained Token**. 
- From the page that opens, choose the token that you use for Digital Garden.

Now this will open the settings page for that *fine grained token* that *Digital Garden* uses. You wil see that the **repository permissions** do not include any repositories.

- Edit it and choose the newly created Digital Garden repository (the deploy repo) and save it.

Now when you go back to your Obsidian and deploy the intro page with **publish single note** you will see that after a few minutes, your intro page will be published. Then you can proceed to publish the multiple notes.