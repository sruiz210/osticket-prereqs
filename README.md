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
<p><b>Step 1. Install / Enable IIS in Windows WITH CGI (World Wide Web Services -> Application Development Features -> [X] CGI)<p><b>
<p>
<img src="https://i.imgur.com/M0C0Ggm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 2. From the installation files, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
<p>
<img src="https://i.imgur.com/u8HFYeI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 3. From the installation files, install the Rewrite Module (rewrite_amd64_en-US.msi)
<p>
<img src="https://imgur.com/WEpbTZK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 4. Create the directory C:\PHP
<p>
<img src="https://i.imgur.com/0m6NqCv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 5. From the installation files unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into C:\PHP file folder that you just created.
<p>
<img src="https://i.imgur.com/9lwCDFx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 6. From the installation files install VC_redist.x86.exe.
<p>
<img src="https://i.imgur.com/Fch3oMY.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 7. From the installation files install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Password1
<p>
<img src="https://i.imgur.com/L4xELKJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
7.b
<img src="https://i.imgur.com/hVCuzlm.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 8. Open IIS as an Admin >register PHP >then restart the server
<p>
<img src="https://i.imgur.com/HUi5Fsb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
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
Step 9. Install osTicket v1.15.8. Copy “upload” folder to c:\inetpub\wwwroot
<img src="https://i.imgur.com/FDUOK13.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
9b. Within C:\inetpub\wwwroot, rename “upload” to “osTicket”
<img src="https://i.imgur.com/SPNfQXq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
Step 10. Go Back to IIS Manager> sites> Default> osTicket and double click on PHP Manager to enable a few extensions.
As shown below there are a few X's next to a couple of disabled extensions. 
<img src="https://i.imgur.com/YgnM7of.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
On IIS manager select " Browse*:80(http)" on the right to check the status of osTicket sytem extensions.
</p>
<p>
</p>
10b. Click "Enable or Disable Extension"> right click and select "enable" on the following extensions; php_imap.dll, php_intl.dll, php_opcache.dll
<p>
<img src="https://i.imgur.com/QfsYQuS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
10c. Once extensions are enabled, refresh the osTicket browser. If done correctly, the browser should look like this.
<img src="https://i.imgur.com/5ysJn3V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
Step 11. After navigating to http://localhost/osTicket/setup/install, rename the ost-config.php file and click continue.
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
<img src="https://i.imgur.com/QHt8q3Q.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Step 12. After changing the ost-config.php file and clicking continue and you should see the following screen:
<img src="https://i.imgur.com/jiztQHW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Fill out the information and click save when finished.
</p>
<p>
</p>
<br />
Step 13. Step 14. From the installation files install HeidiSQL
-Open Heidi SQL
-Create a new session, root/Password1
-Connect to the session
-Create a database called “osTicket”
-Click Open
</p>
Image 1. <img src="https://i.imgur.com/Ah5yrmI.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Image 2. <img src="https://i.imgur.com/2Kqioe1.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Thank you for following along !
</p>
<br />
