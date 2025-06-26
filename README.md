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
- Account Expired
- Password Rest
- File Permission 

<h2>I.T. Issues & Resolutions</h2>

<h3>:lock:User Lockout</h3>

<ins>User Affected:</ins> Kevin Malone </br>
<ins>Admin Resolving Issue:</ins> Kevin Benavides (Domain Admin) </br>
<ins>Description:</ins> Kevin Malone was unable to log into his workstation after exceeding the maximum number of failed login attempts. As a result, his domain account became locked out. </br>
</br>
<ins>Root Cause:</ins> Too many failed password attempts triggered the account lockout policy defined in the domain. 


<img width="767" alt="Screenshot 2025-06-24 at 4 41 38 PM" src="https://github.com/user-attachments/assets/bb2b55e1-0954-45ba-a234-76bef0fd3d21" />

<h3>Resolution:</h3>

https://github.com/user-attachments/assets/99f16579-0f18-4734-a621-9f53ec4db05f

<br />
- Opened Active Directory Users and Computers (ADUC)<br />
- Navigated to the Sales OU<br />
- Right-Clicked on Kevin Malone's account -> selected Unlock Account<br />
- Verified Kevin was able to log in afterward.<br />

<h3>:no_entry_sign:Account Expired</h3>

<ins>User Affected:</ins> Dwight Schrute </br>
<ins>Admin Resolving Issue:</ins> Kevin Benavides (Domain Admin) </br>
<ins>Description:</ins> After returning from vacation, Dwight Schrute was unable to log into his workstation. Investigation revealed that his domain account had expired during his time away, causing the login failure. </br>
<br/>
<ins>Root Cause:</ins> User account in Active Directory was set with an expiration date, which had passed while he was on leave. This setting may have been part of a security policy for temporary users or accidentally left enabled during account setup.

<img width="414" alt="Screenshot 2025-06-25 at 4 38 18 PM" src="https://github.com/user-attachments/assets/1a90635b-6216-49a6-9a5b-140401b860eb" />

<h3>Resolution:</h3>

https://github.com/user-attachments/assets/7b14fd7a-2838-4e53-ad8d-3d7800f3c430

<br/>
- Located Dwight Schrute's user account with Find.</br>
- Opened user properties and navigated to the Account tab.</br>
- Observed that "Account expires" was set to a past date.</br>
- Updated Dwight's account by setting "Account expires" to "Never"</br>
- Also, made it so that Dwight has to reset his password next time he logs in.</br>
- Confirmed successful login. </br>
<br />

<h3>:closed_lock_with_key:Password Reset</h3>

<ins>User Affected:</ins> Michael Scott </br>
<ins>Admin Resolving Issue:</ins> Kevin Benavides (Domain Admin) </br>
<ins>Description:</ins> Michael Scott was unable to log into his workstation. He reported that he had forgotten his password. </br>
</br>
<ins>Root Cause:</ins> User forgot their password. 
</br>
<h3>Resolution:</h3>

https://github.com/user-attachments/assets/69617fb6-83a2-4d84-88d7-8b6b1ed3b19e

<br />
- Located Michael Scott's account in Active Directory Users and Computers</br>
- Right-clicked the user and selected "Reset Password"</br>
- Chose a temporary secure password and enabled "User must change password at next logon".</br>

<h3>:file_folder:File Permission</h3>

<ins>User Affected:</ins>Angela Martin</br>
<ins>Admin Resolving Issue:</ins> Kevin Benavides (Domain Admin) </br>
<ins>Description:</ins> Angela Martin has reported she is unable to access a shared folder named "Accounting" on the network. When attempting to open the folder, she received an access denied message. </br>
</br>
<ins>Root Cause:</ins> Angela is not a member of the Accounting security group in ADUC.

<img width="952" alt="Screenshot 2025-06-26 at 5 01 16 PM" src="https://github.com/user-attachments/assets/743a78d5-175a-4847-99bd-1eb04b683e07" />

<h3>Resolution:</h3>

https://github.com/user-attachments/assets/95465618-4285-40bb-88b9-e0bb876b2f5d

<br />
-Escalated to the Accounting manager for approval if access was business-justified.<br />
- Approved, so I added Angela to the Accounting security group in ADUC.<br />
- Refreshed group membership on her workstation by loging off and loging back in.<br />
- Now, she has access to Accounting file.<br />
<br />

https://github.com/user-attachments/assets/87e389b3-418d-4adc-872b-6ea98e209290


<br />
