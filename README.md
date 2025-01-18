<h1>Active  Directory Home Lab</h1>

 ### [YouTube Demonstration](-)

<h2>Description</h2>
Active Directory Project by Thoriso Maditse

In this project, the goal is to configure a basic Windows networking environment utilizing Active Directory and essential networking services. By building this lab, the focus is to deepen the understanding of Active Directory and general Windows networking concepts.

Project Overview:

Environment Setup:

Tools used: VirtualBox, Windows 10 ISO, and Server 2019 ISO.
Created two virtual machines:
Domain Controller (Server 2019): Configured with two network adapters (one for external internet access and another for the private network).
Client (Windows 10): Connected to the private network and joined to the domain.
Configuration Steps:

Installed Server 2019 and assigned IP addresses for the internal and external networks.
Set up Active Directory on the Domain Controller, created a domain, and configured NAT and routing to allow private network clients to access the internet.
Configured DHCP to automatically assign IP addresses to clients.
Ran a PowerShell script to create 1,000 users in Active Directory.
Testing:

Installed Windows 10 on a second virtual machine and connected it to the private network.
Named the machine "Client 1," joined it to the domain, and successfully logged in with one of the domain accounts.
Metrics:

Users Created: 1,000 domain accounts.
Virtual Machines Configured: 2 (Domain Controller and Client).
Network Types: 2 (External and Private VirtualBox Network).
Services Enabled: Active Directory, DHCP, NAT, and routing.

This environment serves as a foundation for understanding Windows networking and will be utilized for future learning and instructional purposes.

This repository contains steps on how I set up a basic home lab running Active Directory. The setup was completed by following:
A tutorial by Josh Madakor on YouTube.
Additional resources from Professor Messer’s YouTube channel, which were used to learn more about Active Directory and related concepts from A+ course.

<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Server 2019</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)

<h2>Program walk-through:</h2>

<p align="center">
Diagram: <br/>
<img src="https://i.imgur.com/odFfDCU.jpeg" height="80%" width="80%" alt="Diagram"/>
<br />
  Download and install Oracle VirtualBox from the official website.
  https://www.virtualbox.org/wiki/Downloads
  
  Download the Windows 10 and Server 2019 ISO files.
 https://www.microsoft.com/en-us/software-download/windows10ISO   , ,https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019
<br />
Create a new virtual machine for "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Domain controller Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
