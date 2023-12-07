<h1>YParry - Manage Authorization </h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash Shell</b> 
- <b>Diskpart</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through: Setting Appropriate Access Permissions</h2>

<p align="center">
Checking ''projects'' directory and files: <br/>
<img src="https://i.imgur.com/A3PJH42.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Checking Whether Any Hidden Files Exist: <br/>
<img src="https://i.imgur.com/kQNDUcE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Check If any files in the projects directory have write permissions for the owner type of other: <br/>
<img src="https://i.imgur.com/ImTHlQf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change the permissions of the ''project_k.txt'' file so that the owner type of other doesn’t have write permissions: <br/>
<img src="https://i.imgur.com/WwA42CF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
