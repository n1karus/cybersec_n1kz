+++
title = "Reflection 1"
date = "2020-22-01"
author = "Nik"
cover = "/images/reflection1img.jpg"
description = "This is the reflection for sprint 1 :)"
+++

## Reflection:

> When we first started this project on Monday (20/01/2020), the stakeholders are mentioned a few times. The tutors were explaining to us about what static sites were, how they worked,
and how they were secure due to there not being any critical data stored on the actual site. We briefly touched on the first Subject Learning Objectives (SLO) at the start then went on to 
begin the project, where I should have asked more questions to engage and identify the problems in the industry. After the briefing on all the SLOs, I began to install, register, and gather all 
the resources I needed to make the static site for my e-portfolio, namely: Hugo, Netlify, GitHub education pack, git and Namecheap. After registering a domain and setting up Hugo as well as git, 
I began to develop a local static site on my laptop. I spent the entire day at the lab figuring out how to use git (refer to figure 4) through a command-line as I had only used it through GUI 
before. Afterwards, I spent the day generating a local site through Hugo and playing around with the themes for my static site, where I finally chose Terminal (refer to figure 3). After I 
generated the site and made an About Me page, I left to go home.
>
>Unfortunately, I have work on Wednesdays (22/01/2020), so from now on, I won't be able to come into the drop-in sessions. However, at night after work, I had begun to work on my site where I used 
the resource provided in the Microsoft Teams resource page on how to set up a Hugo page using Netlify (https://www.netlify.com/blog/2016/09/21/a-step-by-step-guide-victor-hugo-on-netlify/). 
I had gotten to the point where Netlify points to Github, and everything was set up; however, the deploy was failing. Luckily, Dylan Tchan had gone to the drop-in session today and spent the whole 
day working on getting his site deployed, and after troubleshooting my errors together, we found out he had the same issue (refer to Figure 5). By using the variable that is shown in Figure 6, 
Dylan helped me successfully deploy my domain and Github pages, so all files pushed to git will finally appear under my domain n1kz.me.
>
>In the lab on Thursday (23/01/2020), I was late, but an industry guest (Matthew Brennan) came in to talk to us about the cybersecurity industry, his job, and how he got there. He provided us 
with a lot of pathways on how to get a role in the industry, such as war games or courses we can take that are useful in teaching us about Cyber Security. Thinking back to this meeting, I realised 
I should have asked Matthew more questions about the impact of attacks and common vulnerabilities since he used to be a Penetration Tester since he is a stakeholder within the industry. I should ask
later if I can get his contact details to meet the first SLO. After his talk, we continued with our e-portfolio, where I created an About Me page and a reflection page where I began to upload all
the screenshots I took throughout the process of me creating this static site. During the lab, Tyrone Huang had asked Jason how this whole static site worked as he was confused to which Jason 
created a clear diagram seen in Figure 10, and he explained how the websites are structured and how it communicates through each node. Later on, in the lab, I had tried to redirect my homepage to 
my About me page instead, which ended up not working and resulted in Figure 8. Luckily I had only changed one line and was able to find the source of the problem pretty quickly. I began to research
Hugo documentation and StackOverflow for ways to set the homepage without breaking your site only to find out that to do it, you need to customise your theme and change a few settings. Thus, I 
decided to leave it as one of the Tutor's Jason had told me after that it is okay for my blogs page to be my homepage. Afterwards, a few people in my class were having the same issue of trying to 
change their homepage and breaking their site, which I helped some by telling them to change the line highlighted in Figure 9.
>
>After working the rest of the days, I was finally able to work on my website the whole of Monday (27/01/2020). I had updated my Introduction page and merged it with my About me page, fixed up all 
the screenshots on my reflections page, and made sure all the pages were formatted correctly. However, one thing I feel like I should change in the reflections page is rather than having all the 
screenshots/figures at the bottom one after the other, and I mix the images in with my reflection statement.

## What happened during Sprint 1 screenshots: 

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

![Figure 9](/images/solution2.png)  **Figure 9: Solution 2 - Fixed site theme** 
>On the Thursday (23/01/2020), Tyrone Huang asked one of our tutor's Jason on how the static sites were actually generated and deployed, and how it worked. Jason explained it to us through
the use of a diagram as shown in the image directly below. He showed us how to structure our website and the way it communicates between all the different nodes such as all the files being stored
on github, which is connected to Netlify that grabs the files stored and hosts the webpage hosted under the domain provided by namecheap.  

![Figure 10](/images/sitestructure.jpg) **Figure 10 - Jason's diagram on the structure of sites and how they all communicate** 
