# Project---Microsoft-Active-Directory-
Microsoft Active Directory, Powershell Script automatically creates 1000 user accounts, Domain Controller, DHCP Server, DNS Server, Client PC, Virtual Box, Virtualization

INTRODUCTION

This lab was a fun experience and allowed me to solidify some of the concepts of Microsoft Active Directory and what it really is. I already have experience deploying operating systems using virtualization. (VMWare and VirtualBox). This allowed me to dive in just a little bit more into a Windows Server environment and build a tiny enterprise domain.

![Overview](https://github.com/OmrSanchez/Project--Microsoft-Active-Directory-/assets/54558041/94708324-2e06-44bb-95e6-5a01a19d865c)

My goal here was mainly to reach functionality of both the DC and the Client PC without adding more advanced features. The script is not one I developed, however I can understand what each line means and what is doing. 

The steps I took are below along with a few screenshots.
1.	Run a Windows Server 2019 instance with at least (2) NICs.
![Screenshot 2024-02-16 112413](https://github.com/OmrSanchez/Project--Microsoft-Active-Directory-/assets/54558041/f5f39f5d-e27b-40fb-b901-afb332e5cdb1)
2.	Elevate the server to become a Domain Controller running Active Directory, DHCP, DNS.
![Screenshot 2024-02-16 112326](https://github.com/OmrSanchez/Project--Microsoft-Active-Directory-/assets/54558041/5a9039b6-f5d7-4221-a326-2739ba603529)
3.	Manually create an admin account and assign it to the “DOMAIN ADMIN” group. 
4.	Run a script using PowerShell ISE that automatically will create a new “Organizational Unit”, 1000 user accounts, and assign those accounts to the OU.
![Screenshot 2024-02-16 112501](https://github.com/OmrSanchez/Project--Microsoft-Active-Directory-/assets/54558041/45e944ce-ea81-4c84-a966-2a106d0a5f23)
5.	Create a Windows 10 instance and “join” it to the domain. 
 
Functionality of each process was performed throughout the process. This includes using command prompt and ipconfig /all to verify that the client received the correct IP from the scope, pinging an Internet resource from the client which verifies DNS, logging into to many user accounts that were in the OU.

The link found here shows the finished project. I cover all of the details of the project. There is no audio, however everything is clearly demonstrated.

https://youtu.be/n81yY1qU99U?si=zJPEWJgM7mO4Wlip
