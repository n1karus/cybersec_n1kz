+++
title = "Reflection 4"
date = "2020-02-10"
author = "Nik"
description = "This is the reflection for Week 4 :)"
+++

### Monday (10/02/2020)

> For the Monday class in Week 4 I had come into class late at about 11am. I walked into the latter half of Jason doing a demonstration of hacking a box called wakandaforever. Due to missing the 
> first half of the demonstration I was completely lost and was not able to understand anything that was happening. After the demonstration I told Jason I had not understood and he gave the class 
> a quick verbal run through of the whole process again and told me that a fellow classmate Yukari had recorded the whole demonstration which I decided to watch later.
>
> We were also given our deliverable for this week which was to find a beginner/easy level box, break into it and make a write-up for it by Sunday. It sounded like this week was going to be an 
> intensive week especially since I missed the demonstration but I feel super keen to try breaking into boxes as I always found doing this type of stuff interesting but had no experience in doing 
> it before. To start us off we were told to go to [vulnhub.com](http://vulnhub.com) and start doing a box called Basic Pentesting 1. 
>
> ![Reflection4SS1.png](/images/Reflection4SS1.png) **Figure 1: Write up for Basic Pentesting 1 (n1kz.me/posts/basic-pentesting-1)** 
>
> I started to do a write-up for the box as I was doing it  rather than complete it and do the write-up all at once after I did everything like my Natas and Bandit logs. 
> I figured out although this way of making the write-ups makes the process take longer in actually breaking the box, it is a more effective method. It helps me think about what I just did and
> what I am doing and question if it was the correct steps. It also forces me to stop doing all the work last minute like I usually do and try to remember everything a while after when I write the 
> logs. Thus. I am glad I have started doing the write-ups as I do the activities such as trying to hack into the box as it is a more smooth and efficient process that helps me more than my old habits.
>
> Doing this allowed me to take my time with doing the box at my own pace rather than rushing ahead and I ended up staying back after class for 4-5 extra hours just working on both my write-up 
> skills and breaking into the box. As seen in my write-up at [n1kz.me/posts/Basic-Pentesting-1](http://n1kz.me/posts/Basic-Pentesting-1). I was successfully able to gain root access to 
> the box although taking quite a bit of time working through small difficulties such as the exploit not executing properly which now that I look back I did not include in my writeup properly all 
> my issues with Metasploit. Thus, my goal for this week is to try and write a more technical and fleshed out write-up for the deliverable this Sunday. 
>
> Doing this box however taught me that there are several different ways of breaking into a box and gaining root access as seen in the write-up where I had started off in the correct direction for one of the methods, which was brute forcing and trying out all the common passwords to log into the admin account. I gave up after a few attempts and only at the end did I see that the password was the same as the username which surprised me as I started this whole box in the correct direction, but was not able to quite connect the dots or try other obvious passwords. Hopefully by the end of this summer studio however I can gain proficiency in using tools that help me in this like using **John the Ripper** and etc without having to google which tool to use or how to use it in Kali.

### Tuesday (11/02/2020)

> I decided to attempt Basic Pentesting 1 again today to see if I had actually soaked in the methodologies and was able to execute it again myself to which I was able to easily do by following the 
> process as seen in Figure 2:
>
> ![Reflection4SS2.png](/images/Reflection4SS2.png) **Figure 2: Penetration Testing Lifecycle**
>
> As I was able to redo Basic Penetration Testing 1 by following the life cycle rather than remembering the commands I was quite happy with myself and felt that I did sufficient work in starting 
> the foundation for learning how to pentest. However to further build on that foundation I decided to watch videos so I started off with the video that Yukari took of the demonstration: 
> [https://www.youtube.com/playlist?list=PLI6vqVtN06dVeLYvbLAbYkayfiSeE7drR](https://www.youtube.com/playlist?list=PLI6vqVtN06dVeLYvbLAbYkayfiSeE7drR) and also began on a youtube playlist 
> called "Penetration Testing with Kali Linux | Learn Ethical Hacking" which teaches you the different tools and methods used in Kali for penetration testing 
> ([https://www.youtube.com/playlist?list=PLp4w7b_XLssSa0I4z6-pz_z48e9am14fg](https://www.youtube.com/playlist?list=PLp4w7b_XLssSa0I4z6-pz_z48e9am14fg)). I think today although I did not get much 
> practical work done, I feel like I did sufficient enough work in learning theory and watching relevant youtube videos and re-affirming the knowledge I had learned yesterday by redoing the box 
> Basic Pentesting 1.

### Wednesday (12/02/2020)

> After work I began to try doing the next box in the series called Basic Penetration Testing 2. I followed through the same process as I did before in finding the IP address of the target machine 
> and trying to gather enough information on how I was going to exploit and gain root access. However after trying the whole day I got stuck up to a certain point that I could not figure out how I 
> was meant to get the usernames. I did not know what enumeration was until I finally caved into looking at another person's write-up and figured out that you can enumerate domains to figure out a 
> lot of different information such as share files or usernames. I ended up reading the rest of the write-up rather than attempting the rest of the box myself.
>
> ![Reflection4SS3.png](/images/Reflection4SS3.png) **Figure 3: Write-up for Basic Pentesting 2 ([https://resources.infosecinstitute.com/basic-pentesting-2-ctf-walkthrough/#gref](https://resources.infosecinstitute.com/basic-pentesting-2-ctf-walkthrough/#gref))**
>
> Thus, I felt like I had cheated and did not end up doing a write-up for this particular box. I want to re-attempt this box next week and possibly make a write-up then to see if I can actually 
> complete it on my own rather than just follow another write-up. However I do not think that looking at another write-up for guidance is cheating. But when you just follow the walk through and 
> not just using it to help you past a certain blockade is when I thought it was cheating which I had ended up doing this time. Due to what happened today, I set a proper goal of being able to 
> hack into a box without looking at a write-up for help by the end of the studio, regardless of the difficulty.

### Thursday (13/02/2020)

> We started off our Thursday with the usual stand-up meetings we did where we talked about our strengths, weaknesses and how we are going to work on our weaknesses. I highlighted the weakness I 
> came across yesterday about how I had to refer to a write-up for a box that I did and that I followed it rather than trying to figure it out on my own and only using it as a last-call reference 
> point. However to fix that weakness I am going to research more and do more boxes so I can gain more experience and set the goal of completing a box and a write-up without looking at an already 
> complete write-up/walk-through. 
>
> We then went through another box as a demo but this time as a class where the class would give input on what we do rather than Jason just doing the demo. However the box that we ended up doing 
> as a class was Basic Pentesting 2 which I had done yesterday so I took a step back from helping out as much and only helped when asked to point the class in the right direction. While that was 
> going on I had a quick chat with Max about the box I was choosing for the deliverable which I ended up choosing a box called **UA: Literally Vulnerable** 
> ([https://www.vulnhub.com/entry/ua-literally-vulnerable,407/](https://www.vulnhub.com/entry/ua-literally-vulnerable,407/)). I found out that 2 other people were doing the same box who was 
> Hayden and Matthew which meant I had people I could talk to about the box if I ever ended up getting stuck.
>
> I began trying to break into the box following the process I have learnt and started using reconnaissance tools to gather information first. I did my write-up as I went along again and after 
> reading other people's write-ups on Wednesday,  I feel like I have a better understanding on how technical write-ups are meant to be.
>
> ![Reflection4SS4.png](/images/Reflection4SS4.png) **Figure 4: My Literally Vulnerable write-up in notion ([https://n1kz.me/posts/ua-literally-vulnerable/](https://n1kz.me/posts/ua-literally-vulnerable/))**  
>
> As seen in the beginning of Figure 4, I started to try improve on my write-up skills and flesh it out by explaining my thought process and what was happening at the time and why I chose the IP 
> address I did. I also labelled the screenshot with red text on what commands I used in that instance to make it easier to see what I did and how. I personally think that compared to my previous 
> write-ups such as [n1kz.me/posts/bandit-logs](http://n1kz.me/posts/bandit-logs), [n1kz.me/posts/natas-logs](http://n1kz.me/posts/natas-logs) and [n1kz.me/posts/basic-pentesting-1](http://n1kz.me/posts/basic-pentesting-1) 
> I have began to understand more on how I should be writing them and have improved significantly. Before I was only doing simple lines just specifying the code I used and what I did but for the 
> Literally Vulnerable write-up, which is the deliverable for Sunday I have started to expand more on why I'm using commands and fleshing out the process. 
>
> After working on my box for a bit I had a one on one with Jason and Larry on my progress, how the studio is going and etc. They gave me great feedback on how my reflections have improved 
> significantly and I have been critically self-evaluating myself throughout my reflections meaning I have met a personal minor goal and successfully taken in their feedback from previous weeks on 
> my reflection. However they had mentioned that I had hit all SLOs except for SLO 1 in my Reflection 3 and that tutors counted as stakeholders too. Which I then had a brief discussion with them 
> about how they had mentioned previously about Samba being a platform known for many vulnerabilities. However I misunderstood them and thought Samba was just a really vulnerable platform which 
> Jason then corrected me by saying **"Software is not innately insecure but measures need to be taken to make operation of that software secure"** which I felt was a really good point about the 
> current problems in the cyber security industry and how important security patches are for software. This was further highlighted from what we had been doing this entire week in where we had 
> exploited old versions of software used by ports in boxes such as Basic Pentesting 1. 

### Saturday (16/02/2020)

> I just continued to work on the deliverable and trying to crack into the box **Literally Vulnerable**. Everything seemed to be going smoothly and I was making great progress without any real 
> external assistance. I was able to use my own knowledge that I had gained over the course of this Summer Studio as well as my previous university classes to progress through the box smoothly. 
> As I did the box over the course of the day, I had some discussions with Hayden along the way on how we both were going over Facebook Messenger as we were doing the same box. We discussed the 
> methods we used to get where we currently were in the box and some tips to help each other out.
>
> ![Reflection4SS5.png](/images/Reflection4SS5.png) **Figure 5: Messenger Chatlog with Hayden Drummond about the Box**
>
> However after taking a break and continuing on with the box at night I ended up at a dead-end. The dead-end however was in the sense that I was unable to perform a **wpscan** as seen in Figure 6 
> where it kept on aborting the scan and returning a 403 error.
>
> ![Screenshot_12.png](/litvulnimg/Screenshot_12.png) **Figure 6: wpscan error**
>
> As elaborated on in the Literally Vulnerable write-up, I had spent a significant amount of time trying to fix this issue so I could enumerate the users on the target machine. I had continued to 
> try to figure out the error and fix the problem. I had googled the error however no one else had the exact same error or had a solution that worked, and there seemed to be no tools at all that 
> allowed me to do what I needed to do to progress in the box. I ended up staying up until 5am Sunday morning trying to fix this error by deleting and reinstalling Kali Linux, updating **wpscan** 
> however nothing seemed to work and I gave up and went to bed. I think for this night I had worked and focused way too much on a single error and worked sufficiently in trying to troubleshoot and 
> fix the error itself however despite the time and effort I put in, the problem did not fix itself. This was quite the predicament as I could not think of any other way to continue on with the 
> Box without performing the **wpscan.**

### Sunday (16/02/2020)

> I was pretty tired from waking up after staying up until 5am however I still persisted on trying to go through with the Box and trying to complete it with the limited time I had left. 
> I had continuously tried to delete and redownload Kali and updating it through the shell however nothing worked.
>
> ![Reflection4SS6.png](/images/Reflection4SS6.png) **Figure 7: Messenger Chatlogs with Jason Ko (Tutor)**
>
> After asking Jason Ko on messenger for help he had attempted to give me help in trying to troubleshoot the error however there was nothing that seemed to help and he also agreed that **wpscan** 
> was probably the only tool that could be used for what I needed to progress in the box. Thus, I had given up on trying to waste my time in progressing the box and instead tried refining my 
> write-up for the deliverable as much as possible. I read the example write-up that Jason had posted ([https://nosj.me/Wakanda.pdf](https://nosj.me/Wakanda.pdf)) to see how a technical write-up 
> should be. I saw many details that he included that I never thought of including such as all the tools that he used and what they did and separating the write-up into the different phases of the 
> penetration testing lifecycle.
>
> However overall, for my write-up I think I made a massive improvement on how I presented and typed it up compared to my last write-ups. I think I had worked sufficiently on the write-up itself 
> however I am disappointed that I was not able to complete the box in time for the deliverable due date. I am hoping however to go in on Monday and see if the tutors can help me with the error 
> in class so I can finish the box on my own time and finish the write-up.