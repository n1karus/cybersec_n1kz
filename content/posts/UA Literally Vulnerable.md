+++
title = "UA: Literally Vulnerable write-up"
date = "2020-02-13"
author = "Nik"
description = "This is the write-up for Literally Vulnerable!"
+++

- First thing I did was try to gather information on what IP address the box was using. Going into Kali Linux I discovered 4 hosts but crossed out .1 and .2 straight away as that is the Network 
Address and the 2nd address is usually reserved for the host. The last one so in this case .254 is the broadcast address leaving .130 as the last usable address.

- ![Screenshot_1.png](/litvulnimg/Screenshot_1.png) Command Used: **netdiscover**

- To confirm that .130 was the address I put it into firefox which brought me to a wordpress site confirming its the correct address and that the HTTP port is open and is hosted on a webserver as 
seen in the image directly below:

- ![Screenshot_2.png](/litvulnimg/Screenshot_2.png)

- To continue gathering information and follow the regular process that I've been following in the other boxes such as Basic Pentesting 1 & 2, I performed an nmap on the ports for 
**192.168.93.130** to see the ports that are open and what versions they are to see if there possibly may be any that I would be able to exploit. Once I completed this scan I saw an interesting 
note about the FTP port where it says "Anonymous FTP login allowed". This intrigued me so I began trying to log into FTP.

- ![Screenshot_3.png](/litvulnimg/Screenshot_3.png) Command Used: **sudo nmap -sV -sC -o literallyvulnerable1.log 192.168.93.130**

- I tried logging into FTP using the command **ftp 192.168.119.128 (different IP as I am on a different PC)** however I was given the reply **bash: ftp: command not found.** Not knowing how to log 
into the FTP besides this I gave it a quick google search which told me that I needed to install the packages first. So I used the command **apt-get install ftp** which installed the packages and 
dependencies then used the command **ftp 192.168.119.128** again and prompted me to log in with a username. I logged in with the user: **anonymous** as it said in the nmap scan that anonymous FTP 
login was allowed and successfully logged into the directory which showed the file backupPasswords as seen in the screenshot directly below. Reading the output of the file we see that one of the 
users are called Doe and there is a list of passwords with one of them being the correct one.

- ![UA%20Literally%20Vulnerable/Screenshot_4.png](/litvulnimg/Screenshot_4.png) **Commands used: ftp 192.168.229.128 / ftp > get backupPasswords / cat backupPasswords** 

- Getting the list of backup passwords I had decided to go back to the webpage which was still not loading properly so I checked the developer console (F12) which immediately brought to my 
attention that the site was requesting the domain "**literally.vulnerable"** for an external script to load the page. 

- ![UA%20Literally%20Vulnerable/Screenshot_5.png](/litvulnimg/Screenshot_5.png)

- When I tried clicking on the admin's account from this webpage it was unable to connect to the server or find the site and pointed me to the URL 
"**literally.vulnerable/?author=1"**. So to try and fix this I recalled some knowledge on /etc/. Having done subjects at UTS such as Security Fundamentals, Network Servers and Cyber Security, 
I knew that there was a file in the location **/etc/hosts** that allows you to point a domain to a machine's IP address. 

- ![UA%20Literally%20Vulnerable/Screenshot_6.png](/litvulnimg/Screenshot_6.png) **Commands used: echo "192.168.229.128 literally.vulnerable" >> /etc/hosts**

- Editing the file to point the machine's IP address and the domain name helped fix the formatting and fully loading the page as seen in the screenshot directly above. I then went to the log-in 
screen and automatically began trying to log into the admin account by brute forcing it. I attempted to use the username "admin" as I saw that account have a post and went through all the 
passwords in the file that we got **backupPasswords.** However after manually copy and pasting all of these passwords I was unable to log-in.

- I ended up being stuck at this point and was trying to find out what I could do. I tried using the command **dirb** on the website but found no directories. 
I tried looking for exploits on **[http://exploit-db.com](http://exploit-db.com)** for the port versions however found no relevant exploits that would be of use. I also began seeing if I could 
find a hidden site by going **literally.vulnerable/robots.txt** and etc however to no avail. I was racking my brains to figure out and finally caved into looking at a writeup for just the 
beginning to see what I did wrong to already end up at a seemingly dead-end. However at one of the first few screenshots I realised that the NMAP results of theirs differed slightly in mine in 
where they had an extra open port that you could see. Highlighted in the screenshot below the port 65535 was also open and was hosted on an Apache webserver.

- ![UA%20Literally%20Vulnerable/Screenshot_7.png](/litvulnimg/Screenshot_7.png) Commands used: **nmap -sV -p- 192.168.229.128**

- To stop myself from spoiling this box and so I could figure the rest on my own, I closed the write-up immediately and began investigating further. I went to the port 65535 by attaching it to the 
domain literally.vulnerable:65535 which I learned from all the times I played with making my own minecraft server as a kid. It took me to the default page for Apache2 Ubuntu so I decided to 
<span style="color:red">**dirb**</span> the site as I could not find any other clues from the default landing page.

- Immediately upon **dirb**ing the website with the port **65535** it immediately found me a directory different from the default javascript ones: **/phpcms/.** 
I had used the big.txt file to narrow the search as a default dirb search returned nothing and the first result that appeared on google after searching for "dirb wordlist kali" was big.txt.

- ![UA%20Literally%20Vulnerable/Screenshot_9.png](/litvulnimg/Screenshot_9.png) Commands used: **dirb [http://192.168.229.128:65535](http://192.168.229.128:65535) /usr/share/wordlists/dirb/big.txt**

- Loading into this page showed me a new post that was "Protected: Secure Post" by a user called notadmin and required a password to view. I tried copy and pasting every password into the text 
field again however to no avail. I noticed some posts below however and an interesting one titled "Damn, What should I do?" that gave a big tip as seen in the screenshot below.

- ![UA%20Literally%20Vulnerable/Screenshot_10.png](/litvulnimg/Screenshot_10.png)

- So, as suggested from the post I began trying to enumerate the website to try and find out the different users so I can figure out which one has the password from the list we obtained earlier.

- ![UA%20Literally%20Vulnerable/Screenshot_11.png](/litvulnimg/Screenshot_11.png)

- However, as you may notice when you use the command **enum4linux** it does not allow you to use special characters, thus I figured out that enum4linux only works for IP addresses and cant be used 
for ports or actual website domains. However when I enumerated just the IP address it failed as the server did not allow the use of ' ' in username or password. I googled 
"how to enumerate wordpress usernames" and found out that there was a command that can be used in Kali called **wpscan**. I began trying to use the command to enumerate the WordPress site by using 
**wpscan** however the command did not work properly as it kept aborting the scan as it was "Unable to get https://data.wpscan.org/plugins.json.sha512". Thinking that it was because wpscan was out 
of date I tried to **apt-get install wpscan** which instead of fixing my problem made it worse as whenever I used wpscan it said I did not have the correct ruby dependencies and did not allow me 
to do anything anymore, essentially breaking my box. Thus, I had to redownload the Kali VM, making me realise that making a copy or clone of the VM is quite important. 

- ![UA%20Literally%20Vulnerable/Screenshot_12.png](/litvulnimg/Screenshot_12.png)

- As you can see in the screenshot above, when I initiate the wpscan, it starts updating the database before immediately aborting the scan due to the error. I had googled the error but nothing 
appeared. I had also updated Kali due to Jason's advice but to no avail and tried reinstalling it instead. Yet wpscan had still not worked. I felt really frustrated and at a wall as I spent the 
whole night googling if I could use another tool to enumerate the users or if anyone else had a solution for the error, but found absolutely nothing on Google.