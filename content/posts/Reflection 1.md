+++
title = "Reflection 1"
date = "2020-22-01"
author = "Nik"
cover = "/images/reflection1img.jpg"
description = "This is the reflection for sprint 1 :)"
+++

## Reflection 
> 

## What happened during Sprint 1 : 

> Using the github education pack I got a free domain name name by going into namecheap and registered n1kz.me under me

![Reflection/ScreenshotNC.png](/images/ScreenshotNC.png)  

> Afterwards I installed Hugo, which I was recommended by Jason to use as it is the easiest static site generator out of all the options to use. It required me to go into the commandline and generate some files.

![Reflection/Screenshot1.png](/images/Screenshot1.png)

> After playing around with hugo and using the command 'hugo new site' it generated all the files required for the website. Afterwards I went to https://themes.gohugo.io/ where I picked the terminal theme
 (https://github.com/panr/hugo-theme-terminal/). I deployed the website locally to test the example site which worked.

![Reflection/Screenshot2.png](/images/Screenshot2.png)

> Problem 1

+ Netlify was not able to deploy the website as seen in the error below where the Hugo version was conflicting and outdated on netlify and the theme I was using.

![Reflection/Screenshot3.png](/images/Screenshot3.png)

> Solution 1

+ To fix this error, I asked Dylan Tchan, a fellow student in the Summer Studio for help as he encountered the same problem and after researching for a bit changed the environment variables for 
building/deploying the domain by setting the hugo version to the current version I was actually using.

![Reflection/Screenshot4.png](/images/Screenshot4.png)

> Screenshot of the deployment from Netlify to n1kz.me after pointing it to the github repository.

![Reflection/Screenshot5.png](/images/Screenshot5.png)

> Error 2

+ While trying to change the landing page of my static site through Hugo, I encountered an error where my sites formatting and styling broke completely, only leaving a cached version of the site as seen in the screenshot below.

![Reflection/error2.png](/images/error2.png)

> Solution 2

+ After going through the code, and through researching documentations from Hugo and stack overflow, I had figured out that you are unable to change the landing page of a Hugo site unless you edited the theme or created your own.
 To fix the problem I was having was pretty easy as I was only changing one line which is highlighted in the screenshot below. A few other students in the class, one of them also being Dylan Tchan was having a similar issue, 
and after bringing it up to our tutor's Larry and Jason, we figured out that Hugo did not allow you to change the landing page unless you customised your own theme or the theme allowed it.

![Reflection/solution2.png](/images/solution2.png)


