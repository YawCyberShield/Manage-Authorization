<h1>YParry - Manage Authorization </h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash Shell</b> 

<h2>Environments Used </h2>

- <b>Linux</b> 

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
Verify write permissions for owner or others in projects directory files: <br/>
<img src="https://i.imgur.com/ImTHlQf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Remove write permission from the owner type of other in the ''project_k.txt'' file: <br/>
<img src="https://i.imgur.com/WwA42CF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Comfirm using Is -I   <br/>
<img src="https://i.imgur.com/HbUlFIc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Remove group read permissions from project_m.txt using chmod g-r :  <br/>
<img src="https://i.imgur.com/bt17pxr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set .project_x.txt permissions to read-only for user and group :  <br/>
<img src="https://i.imgur.com/D3zfojq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Remove the execute permission for the group from the drafts directory:  <br/>
<img src="https://i.imgur.com/0Ehxt8t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
