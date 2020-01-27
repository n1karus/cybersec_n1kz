+++
title = "Reflection 1"
date = "2020-22-01"
author = "Nik"
cover = "/images/reflection1img.jpg"
description = "This is the reflection for sprint 1 :)"
+++


## What happened during Sprint 1 : 

> Using the github education pack I got a free domain name name by going into namecheap and registered n1kz.me under me

![Figure 1](/images/ScreenshotNC.png) **Figure 1: Namecheap (nc.me) where you get a free domain as a student** 

> Afterwards I installed Hugo, which I was recommended by Jason to use as it is the easiest static site generator out of all the options to use. It required me to go into the commandline and generate some files.

![Figure 2](/images/Screenshot1.png) **Figure 2: Screenshot of Hugo working in commandline**

> After playing around with hugo and using the command 'hugo new site' it generated all the files required for the website. Afterwards I went to https://themes.gohugo.io/ where I picked the terminal theme
 (https://github.com/panr/hugo-theme-terminal/). I deployed the website locally to test the example site which worked.

![Figure 3](/images/Screenshot2.png) **Figure 3: Test website generated through Hugo**

> I then used Git to push the locally generated Hugo files to my GitHub repository

![Figure 4](/images/ScreenshotGit.png) **Figure 4: Commands used to push to Github**


> Problem 1

+ Afterwards, I had to point Netlify to my github repository which was easily able to be completed as Netlify provided a simple process to connect to your github repository.
 However, Netlify was not able to deploy the website as seen in Figure 5 below where the Hugo version was conflicting and outdated on netlify and the theme I was using.

![Figure 5](/images/Screenshot3.png) **Figure 5: Problem 1 - Error logs of Netlify deployment**

> Solution 1

+ To fix this error, I asked Dylan Tchan, a fellow student in the Summer Studio for help as he encountered the same problem and after researching for a bit changed the environment variables for 
building/deploying the domain by setting the hugo version to the current version I was actually using.

![Figure 6](/images/Screenshot4.png) **Figure 6: Solution 1 - Variable used to fix Problem 1**

> Screenshot of the deployment from Netlify to n1kz.me after pointing it to the github repository, which means that the website was fully functional and successfully deployed online!

![Figure 7](/images/Screenshot5.png) **Figure 7: Successful deployment summary from Netlify**

> Error 2

+ While trying to change the landing page of my static site through Hugo, I encountered an error where my sites formatting and styling broke completely, only leaving a cached version of the site as seen in Figure 8.

![Figure 8](/images/error2.png) **Figure 8: Problem 2 - Cached version of my site**

> Solution 2

+ After going through the code, and through researching documentations from Hugo and stack overflow, I had figured out that you are unable to change the landing page of a Hugo site unless you edited the theme or created your own.
 To fix the problem I was having was pretty easy as I was only changing one line which is highlighted in the screenshot below. A few other students in the class, one of them also being Dylan Tchan was having a similar issue, 
and after bringing it up to our tutor's Larry and Jason, we figured out that Hugo did not allow you to change the landing page unless you customised your own theme or the theme allowed it.

![Figure 9](/images/solution2.png) **Figure 9: Solution 2 - Fixed site theme**

>On the Thursday (23/01/2020), Tyrone Huang asked one of our tutor's Jason on how the static sites were actually generated and deployed, and how it worked. Jason explained it to us through
the use of a diagram as shown in the image directly below. He showed us how to structure our website and the way it communicates between all the different nodes such as all the files being stored
on github, which is connected to Netlify that grabs the files stored and hosts the webpage hosted under the domain provided by namecheap.  

![Figure 10](/images/sitestructure.jpg) **Figure 10 - Jason's diagram on the structure of sites and how they all communicate**

## Reflection

>  When we first started this project, the **stakeholders** were mentioned a few times when the tutors were explaining to us about what static sites were, how they worked and how they were secure due
to there not being any important data stored on the actual site. We briefly touched on the first Subject Learning Objectives (SLO) at the start then went on to begin the project, where I should have asked more questions about
the problem to try and identify problems in the industry. On the Thursday (23/01/2020) I was late but an industry guest (Matthew Brennan) came in to talk to us about the cyber security industry. 
Where, looking back again I should have asked him more questions about the impact of attacks and common vulnerabilities as he used to be a Penetration Tester.Thus, for the first sprint 
I have not met the requirement for the first SLO as I have not engaged enough with the stakeholders to identify any
problems in the industry.
>
>However, in regards to **applying technical skills to develop, model and/or evaluate designs** (the third SLO), I have met it to a certain extent through the creation and deployment of the static
site I am currently building for my e-portfolio for this studio. As seen from the steps of **Figure 1 - 10** above, I have applied **technical skills to develop and model** the e-portfolio. But,
I do not believe I have fully met the SLO, only partially. 


