# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machines
- PHP Manager
- MySQL
- osTicket (Help Desk Ticketing System)
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/M0C0Ggm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1. Install / Enable IIS in Windows WITH CGI (World Wide Web Services -> Application Development Features -> [X] CGI)
</p>
<br />

<p>
<img src="https://i.imgur.com/u8HFYeI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2. From the installation files, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)


</p>
<br />

<p>
<img src="https://imgur.com/WEpbTZK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3. From the installation files, install the Rewrite Module (rewrite_amd64_en-US.msi)
</p>
<br />
<p>
<img src="https://i.imgur.com/0m6NqCv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4. Create the directory C:\PHP
</p>
<p>
<img src="https://i.imgur.com/9lwCDFx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 5. From the installation files unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into C:\PHP file folder that you just created.
</p>
<p>
<img src="https://i.imgur.com/Fch3oMY.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 6. From the installation files install VC_redist.x86.exe.
</p>
<br />
<p>
<img src="https://i.imgur.com/L4xELKJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 7. From the installation files install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Password1
</p>
<br />
<p>
7.b
<img src="https://i.imgur.com/hVCuzlm.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img src="https://i.imgur.com/HUi5Fsb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 8. Open IIS as an Admin, register PHP, then restart the server
</p>
<br />
<p>
8b. The PHP file will be located in the C:\PHP folder previously created. Select the file within named "php-cgi".
<img src="https://i.imgur.com/rsWi9tj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8c. On the right, click "restart" under Actions> Manage server <img src="https://i.imgur.com/RMOHn6d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<br />
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
