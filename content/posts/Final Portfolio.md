+++
title = "Final Portfolio for Summer Studio 2020"
date = "2020-03-02"
author = "Nik"
description = "This is my final portfolio for Summer Studio 2020!"
+++

## Introduction

> My name is Nicholas Zay, and I am currently a 3rd Year student studying a Bachelor of Science in Information Technology at the University of Technology Sydney (UTS). Currently, I do not have a 
> career in the field of IT. Still, I am aspiring to work in the area in the future, specifically in the Cyber Security industry, but had no technical skills or confidence in myself whatsoever. 
> However, by participating in Summer Studio C, I was able to develop my foundational knowledge, skills, and confidence when completing challenges such as CTFs or boxes. In this final portfolio, I 
> will provide insight on how I was able to meet the five Subject Learning Outcomes (SLO) throughout the studio.

### SLO 1 - Engage with stakeholders to identify a problem

> At the beginning of this studio I was perplexed about how to engage and meet with SLO 1 as other studios seemed to have a theme that focused on a singular problem statement where they develop a 
> solution. However, for the Cyber Security studio, there was not a single problem, and every week we were presented with different problem statements and solutions.
>
> Over the six weeks of Summer Studio, we engaged with multiple stakeholders that allowed us to continuously develop problem statements and expose ourselves to the underlying problems in the field 
> of Cyber Security from the very beginning. However, in weeks 1 and 3, I did not interact with any stakeholders as I had assumed that the stakeholders were only the industry guests that came into 
> the studio. But, the tutors for the studio count as stakeholders.
>
>The stakeholders that I had engaged with were:
>
> - Tutors: Larry, Jason, and Max (Week 1-6)
> - Patrick Kelso from UTS Security team (Week 2)
> - Robert Mitchell (Week 2)
> - Pieter Westein and Nathan Jones from the Deloitte Cyber Attack Team (Week 5)
>
> While engaging with all these stakeholders, the main problem I had identified from engaging with stakeholders and hacking into boxes such as OpenAdmin and Traverxec was the issue with outdated 
> software patches having security vulnerabilities. A problem statement that I had got from discussing with my tutor Jason was that "**Software is not innately insecure, but measures need to be taken to make the operation of that software secure**."
>
> Throughout the studio, as I was finding exploits on the internet relatively quickly when doing security challenges such as boxes, it further emphasised the point that the industry stakeholders 
> were making; that the constant updating and patching of the software* after its release is vital. If you do not do these continuous updates, security vulnerabilities from the most straightforward 
> bugs can be found and easily exploited, causing massive damage depending on the nature of the software, for example, the various vulnerable machines that I had hacked into throughout the studio. 
> Most of them had outdated software that I was able to easily find exploits online that led to me being able to gain a foothold into the system and ultimately become root (a.k.a the owner of the 
> system). This allowed me to do whatever I wanted with the machine-like finding credit card details stored onto the machine, which could cause massive economic and reputational damages/impacts 
> that significantly affect the stakeholders of the business.

### SLO 2 - Apply design thinking to respond to a defined or newly identified problem

> When I first started the studio, I had little to no exposure or knowledge in Cyber Security. This contributed to me having issues in applying design thinking appropriately in the early stages of 
> the Summer Studio. However, by practicing on several vulnerable boxes that simulated machines in the real world, I was able to develop an awareness of the types of vulnerabilities, there were in 
> a system and how I should approach them. By continuously practicing on boxes such as Basic Pentesting and OpenAdmin, it moulded the design thinking process I had when approaching these machines 
> and how it generally fits under the Penetration Testing Lifecycle.
>
> ![Final%20Portfolio/FP2.png](/images/FP2.png) **Figure (SLO) 2.1: Penetration Testing Lifecycle**
>
> From doing all these challenges, I was able to use the three major E's: **E**numerate, **E**xploit, **E**scalate when approaching most boxes. By continually going through a cycle of those three 
> E's, I was able to gain hold of a proper design thinking process that allowed me to focus on what I needed to do throughout trying to complete security challenges and incorporate the three E's 
> within them. That design thinking process focused on:
>
> 1. **Enumeration** (Reconnaissance/Threat Modeling & Vulnerability Identification): Enumerating services and OS of the target machine to find possible targets for exploits
> 2. **Exploiting** (Exploitation): Finding and testing an exploit you found for an out of date service that you have enumerated to see if it would work or if extra information can be found
> 3. **Escalating** (Exploitation): Using the exploit on the target machine to escalate your privileges to root such as getting a root shell from a bug in the service
>
> Following these three big E's to systematically gain root on several machines, further highlighted the impacts that businesses using outdated software can have. Being able to gain root ultimately
> means that you have become the owners of a machine and do whatever they want, causing negative financial and reputational impacts on the business if, for example, all their customer data was 
> leaked. This further strengthened my perspective on the importance of software staying updated and helped construct my problem statement.

### SLO 3 - Apply technical skills to develop, model and/or evaluate design

> Throughout the studio, I was continually applying technical skills that I was continuously evolving to meet the deliverables of each week and achieve root access on boxes that I chose to hack. 
> My weekly reflections go into detail about what I did but here is a list of what I did which required the application of technical skills:
>
> - [Week 1:](https://n1kz.me/posts/reflection-1/)
>    - Setting up this e-portfolio static website to document all my attacks and blog my reflections
> - Techniques/tools applied:
>    - Git
>    - Hugo
>    - Netlify
> - [Week 2](http://n1kz.me/posts/reflection-2/):
>    - Begun doing the **[BANDIT](https://overthewire.org/wargames/bandit/)** overthewire wargame (evidence can be found [here](https://n1kz.me/posts/bandit-logs/).) which focused on essential Linux command usage/CLI
> - Techniques/tools applied:
>    - Network Mapper (Nmap) - for presentations in week 2
>    - Linux CLI and command usage for bandit wargame.
> - [Week 3](http://n1kz.me/posts/reflection-3/):
>    - Web app pentesting was done on **OWASP Juice Shop app** challenges (evidence can be found in my third reflection [here](http://n1kz.me/posts/reflection-3)) as well as another overthewire wargame focusing on web app pentesting called **[NATAS](https://overthewire.org/wargames/natas/)**
> - Techniques/tools applied:
>    - SQL Injection
>    - Stored XSS
>    - Burpsuite
> - [Week 4](http://n1kz.me/posts/reflection-4/):
>    - Completed beginner level machines **[Basic Pentesting 1](http://n1kz.me/posts/basic-pentesting-1/)**, **Basic Pentesting 2** (evidence for two only in the reflection [here](http://n1kz.me/posts/reflection-4/)) as well as nearly completing **[UA: Literally Vulnerable](http://n1kz.me/posts/ua-literally-vulnerable/)** on [Vulnhub](http://vulnhub.com/) to get a better feel for penetration testing.
> - Techniques/tools applied:
>    - Linux CLI
>    - Nmap scanning
>    - Directory enumeration (dirb)
>    - Using Metasploit to use exploits
>    - User enumeration through wpscan
> - [Week 5](http://n1kz.me/posts/reflection-5/):
>    - Completed the [HacktheBox invite challenge](http://hackthebox.eu/invite/), attempted a box provided by Deloitte that was named readme. Also completed an easy to intermediate difficulty machine on [HackTheBox](http://hackthebox.eu/) called **Openadmin**. However, due to OpenAdmin being an active machine, I am unable to post the solutions publically due to the HackTheBox Terms of Service.
> - Techniques/tools applied:
>    - Nmap scanning
>    - GitTools
>    - Directory enumeration (dirb)
>    - Deploying a non-interactive shell using a bash script
>    - Privilege escalation with Curl
>    - Privilege escalation by searching directories
>    - Netstat to listen in on ports
>    - Using python scripts to hash keys into a readable format
>    - John The Ripper to brute-force passwords
>    - Exploiting sudo privileges on nano to deploy an interactive shell as root
> - [Week 6](http://n1kz.me/posts/reflection-6/):
>    - Completed the easy-to-intermediate [HackTheBox](http://hackthebox.eu/) machine called **Traverxec**. Since this is an active machine, I am unable to post the solutions publically due to the HackTheBox Terms of Service.
> - Techniques/tools applied:
>    - Nmap scanning
>    - Directory enumeration (dirb) which turned out to be redundant in this box
>    - Deploying a reverse shell using netcat and python
>    - Privilege escalation by searching directories
>    - tar to extract and unarchive files through CLI
>    - Using python scripts to hash keys into a readable format
>    - John The Ripper to brute-force passwords
>    - Privilege escalation by exploiting journalctl to spawn a root-level interactive shell
>
> To achieve my deliverables and gain root access on these boxes/challenges simulating vulnerable machines, I was required to learn and execute technical skills as I completed each one. I feel 
> that throughout the studio, I have extensively developed my skills and learnt how to apply them as I had never attempted a box before this studio. Having not tried a single box, to have gained 
> root access on five different machines by the end of this studio is evidence of massive personal progress and has bolstered my confidence in applying these technical skills to continue trying out
> more machines.

### SLO 4 - Demonstrate effective collaboration and communication skills

> This studio heavily focused on collaboration and communication skills, even with the deliverables that had to be completed individually. I immensely value these two skills as they play a massive 
> role in all aspects of life and especially in the industry, as it is not a one-person effort but rather an effort of a team communicating their issues and how to solve it throughout a project. 
> In the Cyber Security industry, effective communication and collaboration skills are vital as you will need to be able to convey the technical content of security vulnerabilities in layman's 
> terms for the non-technical people in the company, e.g., members of an executive board. This skill allows the non-technical to understand the seriousness, impacts, and risks that these 
> vulnerabilities would cause to the company if they are not remediated.
>
> In the earlier stages of this studio we were tasked with creating two different presentations on a pre-determined topic in the cybersecurity field. We had to make a separate team for each 
> presentation and was forced to collaborate with people we didn't know for our second presentation. However, these presentations and team shuffling promoted us to adapt to new environments, learn 
> new content as we teach others in the class about it, and develop our collaboration skills to try and work as effectively with people we had never worked with before. The two presentations that 
> were made were:
>
> - Topic: Reconnaissance Tools
>    - **NMAP** - Dylan, Hayden, Lachlan and I (Presentation slides are [here](https://drive.google.com/file/d/1OGVWStbooo0fjDjmC5pDpAgAJLfHu36C/view?usp=sharing))
> - Topic: Web Application Pentesting Exploit
>    - **XSS** - David, Matthew and I (Presentation slides are [here](https://docs.google.com/presentation/d/1DuhJOa27AdHdk-1O39FF8xij3knH5nAMjYlQgaupNck/edit?usp=sharing))
>
> My central platform of communication for these two presentations were Facebook Messenger and Microsoft Teams. As both these presentations were short-term projects, we did not bother with trying 
> to use organising platforms like Trello and instead just made plans through messages, which was more than enough. We were able to make calls over Microsoft Teams to communicate and collaborate 
> more effectively while being able to give constructive feedback on each person's work. Evidence of collaboration work for these two group presentations are within my weekly reflections for Week 2
> and 3.
>
> On top of working on the two presentations, I had also collaborated with Dylan, Hayden, and Tyrone on doing the final showcase for our deliverable in Week 6. Rather than use a messaging platform,
> we had performed more face-to-face meetings and worked on how we were going to allocate the showcase and playoff each other.
>
> ![Final%20Portfolio/Reflection6SS5.jpg](/images/Reflection6SS5.jpg) **Figure (SLO) 4.1: Presenting in the showcase to two guests**

### SLO 5 - Conduct critical self and peer review and performance evaluation

> Before this Summer Studio, I had never really taken any attention or cared for critical self-evaluation, or kept any form of a journal or set of goals. Throughout the studio, however, we were 
> forced to keep a journal where we do weekly reflections. We were given continuous feedback from the studio tutors in the form of one on ones. This personal feedback from the tutors helped give 
> me an external perspective on the underlying weaknesses that I had and how to help combat them. This was a good indicator of my progress throughout the studio, as the tutors consistently gave me 
> feedback and continuously made me aware of how I had remediated my previous mistakes.
>
> ![Final%20Portfolio/FP1.png](/images/FP1.png) **Figure (SLO) 5.1: Week 3 Reflection feedback**
>
> The critical feedback that Jason had given on each week's reflection helped strengthen my performance throughout the studio, as he made sure to prod us in the correct direction and re-affirmed our progress, showing us that our efforts were being recognised. Doing these weekly reflections and getting feedback on each one helped me establish a new perspective of myself, as I was beginning to identify weaknesses and question what I had done throughout the week. It allowed me to re-evaluate myself and always question if I was putting in the effort for this studio, which led to me finally to begin setting goals for myself as advised by Jason in Figure 5.1. By continually reflecting on my activities and my self, I was able to focus on the flaws that became more evident such as the lack of time management which, when I focused on improving, allowed me to exert more effort in studio work.
> In this studio, another thing I was introduced to was the concept of stand-up meetings, which we performed at the start of every tutorial. This helped all the students form a connection to each other, as we all voiced our strengths, weaknesses, struggles, and goals for the week. These stand-up meetings had helped me personally as every day, and I would seriously contemplate what I had happened throughout the week in terms of strengths, weaknesses, and how I would remediate them.
> With the use of the weekly sprint reflections, the ongoing feedback from studio tutors, and the daily stand-up meetings, I felt that I was able to conduct critical self-review and evaluation successfully. These three methods allowed me to reflect and improve on myself throughout the studio continuously.

## Conclusion

> When I started this studio, I had gone in with little to no technical background or knowledge at all besides the low amount of content that I had learnt from the UTS security subjects. In my learning contract, I had set some goals that I wanted to complete by the end of the studio:
>
> - Have a solid foundation of skills and knowledge that I can build upon after the end of the studio
> - Be confident and capable enough to take certifications such as OSCP
> - By the end of this studio, have a blog detailing all my challenges and achievements in the IT field
>
>Regardless of my non-existent technical background besides what I had done at university, I had found that the studio allowed me to develop my confidence and technical skills gradually. 
> They had provided the necessary resources that allowed us to learn new content and immediately gave us deliverables every week to challenge us and directly apply what we learnt. This cycle of 
> continually solving problems and trying to learn new things to address new issues helped strengthen my foundation and rapidly developed my skills. I had gone from not having touched or known 
> about boxes that simulated vulnerable machines to have gained root access to 5 different boxes and having the confidence to try more boxes on my own. Thus, ticking off the first goal I had set as
> I believe that I indeed have been able to build a solid foundation of both skills and knowledge that will allow me to continue learning and completing boxes in my own time after the studio. 
> However, for now, even though I do feel confident enough in being able to learn continuously, I do not think I am capable enough to try for certifications such as OSCP yet.
>
> One thing I had never seen coming was how much I enjoyed making an e-portfolio that blogged all my challenges and achievements. Before the studio I had never really wanted or was bothered to make a blog or do write-ups. Being able to set up a working website in under a week and having a medium that details all my achievements, challenges, and work has become a big part of this studio for me. I hope to continue completing HackTheBox challenges, and continue making write-ups for it on my blog, meaning that I have satisfied the third goal that I had when coming into this studio.
>
> Thus, I can confidently say that this studio has helped develop and shape myself and given me proper exposure to the cybersecurity industry. I know for a fact that the valuable insights and skillsets that I have obtained from participating in this studio will help me in my journey in becoming apart of the industry. The studio has given me a clearer vision of my future on wanting to be involved in some form of Penetration Testing as a job. Despite ending the studio here, I hope to continue the process of learning and building upon the foundation that I have constructed into the far future.