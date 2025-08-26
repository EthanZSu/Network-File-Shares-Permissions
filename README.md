# Network-File-Shares-Permissions



This lab focuses on file shares & permissions between an administrator user and other users in Active Directory.  <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)
- Windows Server 2022 Datacenter

<h2>List of Prerequisites</h2>

 1. Virtual Machine "DC-1" (Domain Controller with Active Directory)
 2. Virtual Machine "Client-1" (joined to Domain Controller)


<h2>Lab Experiment Phases</h2>

 1. With an Admin Account: Create File Shares and Permissions.
 2. With a Regular Account: Test the File Share Access.

<h2>Actions and Observations</h2>
<p>
<h3>1. With an Admin Account: Create File Shares and Permissions. </h3>
<img src="https://github.com/user-attachments/assets/aa5bc1e2-4ece-45fe-a763-15c6c51f5d05" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In Microsoft Azure search: Virtual Machines & select DC-1 VM.
 <br />
Copy DC-1's Public IP address into the Remote Desktop Connection & Connect.
 <br />
Enter the administrator account credentials for the VM: your domain administrator account & password.
 <br />
 <br />
Select "Yes" to the Remote Desktop Connection Pop-up.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/800a6ec0-67d7-490b-872a-ab8f791355b4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In DC-1's taskbar search box, search for "File explorer".
 <br />
On the left select: This PC.
 <br />
Then select: Windows(c:) .
 
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/58127844-ad2f-4354-ae97-8717cc4d987d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Beneath the folders, right-click.
 <br />
Select: New, then select: Folder.
 <br />
Title the folder: read-access .
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/830daab6-8791-4861-820b-14a756d6ae97" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click: read-access.
 <br />
Select: properties.
 <br />
At the top select: sharing.
 <br />

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/f13cc8b6-e466-42d9-9fad-5d3244a0913c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click: Share,
 <br />
Input: Domain Users,
 <br />
Click: Add,
 <br />
Click: Share, Done, Close.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/f2d834c6-c35e-43d4-90ef-952e0fa3355c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Beneath the folders, right-click.
 <br />
Select: New, then select: Folder.
 <br />
Title the folder: write-access .
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/2e63d83d-e64c-430a-9286-852fbe3df190" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click: write-access.
 <br />
Select: properties.
 <br />
At the top select: sharing.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/e44b28d9-7def-43a8-9c31-3c2d76f73c4c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click: Share,
 <br />
Input: Domain Users,
 <br />
Click: Add,
 <br />
Change Permission Level to: Read/Write.
 <br />
Click: Share, Done, Close.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/9a070866-d676-473f-b15d-1bf27c989c5e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Beneath the folders, right-click.
 <br />
Select: New, then select: Folder.
 <br />
Title the folder: no-access .
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/50b95691-2b47-4ca5-a3c0-54ec236b33ff" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click: no-access.
 <br />
Select: properties.
 <br />
At the top select: sharing.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/02d476e0-1e57-4047-a887-9d91cea1de6c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click: Share,
 <br />
Input: Domain Admins,
 <br />
Click: Add,
 <br />
Change Permission Level to: Read/Write.
 <br />
Click: Share, Done, Close.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />

<h3> 2. With a Regular Account: Test the File Share Access.</h3>
<img src="https://github.com/user-attachments/assets/068d96d5-0d33-4a88-a640-c1d40690e877" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Server Manager via the taskbar search bar.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/02981e9a-bf11-4606-91cf-8fee8981ecc2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select: Tools on the top right.
 <br />
Select: Active Directory Users and Computers
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/be0093c1-de13-4bbc-a893-c7827afba779" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select a user.
 <br />
Copy the username.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/bd3df1f1-6f79-47ac-b2c5-6c18cf45bb9f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In Microsoft Azure search: Virtual Machines & select Client-1 VM.
 <br />
Copy Client-1's Public IP address into the Remote Desktop Connection & Connect.
 <br />
 <br />
Select: More choices.
 <br />
Select: Use a different account.
 <br />
Paste and sign into the user account & use: Password1 .
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/0cb7df0f-80f6-4700-af69-b8272adc2d72" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "Yes".
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/ff1819e5-ef90-4584-85f4-5002cd5c51ef" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Explorer on the taskbar.
 <br />
In the top searchbar, search for \\dc-1 .

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/3f7a45cc-2075-4433-9b40-945cb1ff1714" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If this account tried to access the "no-access" file on the Domain Controller,
 <br />
this user would find he/she is unable to.
 <br />
 <br />
This outcome makes sense as only Domain Admins were given Read/Write permissions.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/242c53d5-8949-468e-848c-5b51bcae89b4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If this account tried to access the "read-access" file on the Domain Controller,
 <br />
this user would be able to.
 <br />
 <br />
If this user tried to leave a text document inside the file:
 <br />
(by: right-click, New, Text Document)
 <br />
the user would be blocked from doing so.
 <br />
 <br />
This outcome makes sense as Domain Users were only given permission to read the file.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="https://github.com/user-attachments/assets/e2d93267-e3ab-4551-9aee-a1b7dc8f3059" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If this account tried to access the "write-access" file on the Domain Controller,
 <br />
this user would be able to.
 <br />
 <br />
If this user tried to leave a text document inside the file:
 <br />
(by: right-click, New, Text Document)
 <br />
the user would also be able to.
 <br />
 <br />
This outcome makes sense as Domain Users were given Read/Write permissions.
</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />
