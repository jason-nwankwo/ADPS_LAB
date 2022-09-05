# Active-directory-lab

In this lab, I created an Active directory environment using Oracle virtual box. I installed Windows Server 2019 in a virtual machine to be used as the Domain Controller, which houses Active Directory.

I gave this virtual machine 2 Network adapters. One to connect to my home network, and the other to connect to the private/virtual lab network. Following this, I then assigned the IP address to both network adapters.

Next, I installed Active Directory and created a domain, then setup NAT so that clients can get to the internet. Afterward, I setup a DHCP server so that when I create a Windows 10 machine, it can automatically get an IP Address.

Lastly, I ran a powershell script that will create about 1000 users in Active Directory on the domain controller. After creating the users, I created another virtual machine with a network adapter that will attach to the internal network. I installed Windows 10 on this VM to ensure it automatically gets a proper IP address from the DHCP server.

To check the network works, I joined the domain with this computer to log into it with one of the accounts I created, which basically concluded the lab.

A demonstration on my home lab: https://youtu.be/ghLCwL0125c
