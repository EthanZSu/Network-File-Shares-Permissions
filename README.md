# Network-File-Shares-Permissions
<p align="center">
<img src=" " height="70" width="110" alt="Disk Sanitization Steps"/>
</p>


This lab focuses on file shares & permissions, along with security groups between an administrator user and other users in Active Directory.  <br />



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
 3. With an Admin Account: Create a Security Group With Permissions.
 4. With a Regular Account: Test the Security Group Access.

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


<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />


<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
________________________________________________________________________________________________________________________
<br />
<br />
<br />
<br />
