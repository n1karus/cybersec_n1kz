+++
title = "Natas Logs"
date = "2020-02-08"
author = "Nik"
description = "This is my logs for OvertheWire Natas wargames."
+++

### Natas0

> Inspected element of the page
> Checked the div container of the text "You can find the password for the next level on this page"
>
> **password: gtVrDuiDfck831PqWsLEZy5gyDz1clto**
>
> ![natas0.png](/natasimg/natas0.png) **Figure 1: Natas0**

### Natas1

> "**You can find the password for the next level on this page, but rightclicking has been blocked!"**
> My inspect element was already opened when I swapped over to Natas1 which meant that I just passed the level straight away
>- However if you wanted to inspect HTML without right clicking you just press the key **F12**
> **password: ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi**
>
> ![natas1.png](/natasimg/natas1.png) **Figure 2: Natas1 password**

### Natas2

> In inspect element there was an image file located under a div tag

    <img src="files/pixel.png"> == $0

> I tried going into the image file by using the link [natas2.natas.labs.overthewire.org/files/pixel.png](http://natas2.natas.labs.overthewire.org/files/pixel.png) and was trying to see if the password was in the pixel by zooming in. After tryign to find hex converters and everything I finally figured out you are just meant ot go into natas2.natas.labs.overthewire.org/files and go into the users.txt file to find the password.
> password: sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14

### Natas3

> The page looked identical to the previous page, so after entering Inspect Element I saw a suspicious comment in HTML

    <!-- No more information leaks!! Not even Google will find it this time... -->

> Seeing the last part of the comment I naturally looked at how Google find things which led me to learning about automated programs such as spiders and crawlers. This led me to a file called robots.txt that tells crawlers what pages or files the engine can take. So I went to access robots.txt which led me to the webpage in Figure 3.
>
> ![natas3.1.png](/natasimg/natas3.1.png) **Figure 3: Natas3 robots.txt file**
>
> The disallow part looked like a link so I typed that into the url which led me to a directory with a textfile in it that had the username and password to access the next level.
>
> **password: Z9tkRkWmpt9Qr7XrR5jWRkgOU901swEZ**

### Natas4

> **Access disallowed. You are visiting from "" while authorized users should come only from "[http://natas5.natas.labs.overthewire.org/](http://natas5.natas.labs.overthewire.org/)"**
>
> After using BurpSuite to intercept and forward the HTTP request then refreshing the page it changed from the message above to the one in Figure 4.
>
> ![natas4.1.png](/natasimg/natas4.1.png) **Figure 4: NATAS4 landing page after using BurpSuite**
>
> After forwarding the packet and continuing to forward the packet I realised that in the text field on BurpSuite, there was a line with the title **Referrer** that had the exact same url in it as Figure 4, "http://natas4.natas.labs.overthewire.org/".
>
> ![natas4.2.png](/natasimg/natas4.2.png) **Figure 5: NATAS4 using Burpsuite to intercept the request**
>
> I changed the url to match the same one as Figure 4 where it says users should only come from "http::/natas5.natas.labs.overthewire.org/" which granted me the **password: iX6IOfmpN7AYOQGPwtn3fXpbaJVJcHfq**