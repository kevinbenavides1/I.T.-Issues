<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory: Common I.T. Issues & Resolutions</h1>
This section highlights real-world I.T. issues faced in domain environments and how they were resolved using Active Directory tools, Powershell, and standard troublshooting practices.<br />

<p>
  
![The_Office-logo](https://github.com/user-attachments/assets/f27f9f4c-a809-41f6-b94a-67bb32656b4b)
</p>
Will be solving I.T. issues for The Office, a new paper company that has moved into Columbus, Ohio!




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Issues Presented at Work Today</h2>

- User Lockout
- Step 2
- Step 3
- Step 4

<h2>I.T. Issues & Resolutions</h2>

<h3>:lock:User Lockout</h3>

<ins>User Affected:</ins> Kevin Malone </br>
<ins>Admin Resolving Issue:</ins> Kevin Benavides (Domain Admin) </br>
<ins>Desctiption:</ins> Kevin Malone was unable to log into his workstation after exceeding the maximum number of failed login attempts. As a result, his domain account became locked out. </br>
</br>
<ins>Root Cause:</ins> Too many failed password attempts triggered the account lockout policy defined in the domain. 

<p>
<img width="767" alt="Screenshot 2025-06-24 at 4 41 38 PM" src="https://github.com/user-attachments/assets/bb2b55e1-0954-45ba-a234-76bef0fd3d21" />
</p>
<h3>Resolution:</h3>

https://github.com/user-attachments/assets/99f16579-0f18-4734-a621-9f53ec4db05f

<br />
- Opened Active Directory Users and Computers (ADUC)<br />
- Navigated to the Sales OU<br />
- Right-Clicked on Kevin Malone's account -> selected Unlock Account<br />
- Verified Kevin was able to log in afterward.<br />

<h3>Next</h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
