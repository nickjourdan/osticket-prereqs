<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services (ISS)
- Install Web Platform Installer
- Install MySQL
- Install C++ Redistrutible 
- Configure Permissions and Install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/7rR0Sab" height="80%" width="80%" alt="CGI process"/>
</p>
<p>
First, go to control panel, and select programs. From there, click turn windows features on or off. Enable Internet Information services, then expand that program. Enable World Wide Web Services, then expand that program as well. Proceed to expand the Application Development Features program, and finally enable CGI.
</p>
<br />

<p>
<img src="https://imgur.com/a/aQpnp6d" height="80%" width="80%" alt="Download Programs"/>
</p>
<p>
Proceed then to download and install PHP Manager for IIS, as well as downloading the rewrite module.
</p>
<br />

<p>
<img src="https://imgur.com/a/krm04mD" height="80%" width="80%" alt="Folder Setup"/>
</p>
<p>
Create a folder in the C: aree in your pc, and create a folder called "PHP." then proceed in install the file php-7.3.8-nts-Win32-VC15-x86.zip and then unzip the file within the PHP folder. 
</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Download both VC_redist.x86.exe as well as MySQL 5.5.62 programs. When in the MySQL setup wizard, choose the standard configuration.
</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Open Internet Information Services (IIS) and run as administrator. Open up the PHP manager, and register a new PHP version. Link it to php-cgi.exe within he files on the C: files. Restart the IIS once it's complete.
</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Proceed to download osTicket, and then move the upload folder into c:\inetpub\wwwroot. Once there, rename the upload folder to osTicket.
</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Return to IIS and ouble click on PHP manager. From there, click on "Enable or disable extension". Once you get to that screen enable three extensions: Enable: php_imap.dll, Enable: php_intl.dll, Enable: php_opcache.dll.

</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Return to IIS and ouble click on PHP manager. From there, click on "Enable or disable extension". Once you get to that screen enable three extensions: Enable: php_imap.dll, Enable: php_intl.dll, Enable: php_opcache.dll.

</p>
<br />

<p>
<img src="https://imgur.com/a/NFjNuVi" height="80%" width="80%" alt="More Program Downloads"/>
</p>
<p>
Rename ost-config.php from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
to C:\inetpub\wwwroot\osTicket\include\ost-config.php. After that, go to ost.config.php in the file manager, and click properties. Go to security, and disable inheritance; remove all users from it. Then, add new permissions, and type "Everyone" in the users bar, and check all the boxes for full control to all users. Click apply and then ok to finalize changes.

</p>
<br />



