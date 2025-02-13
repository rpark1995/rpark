# rpark
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro (2 vCPU's)</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- Link to downloads: https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Installation Steps</h2>

<p>
1. You will begin by creating a Windows 10 virtual machine in Azure. First, navigate to https://portal.azure.com/. Make sure to select Windows 10 Pro version 22H2 as your image. You want to make sure that your virtual machine contains at least 2 vCPU's and 16 GB of memory to prevent slowdowns.
  </p>
<p>
2. Once you created your virtual machine, you will access it remotely from your personal workstation. Go to the start menu on your personal workstation and type Remote Desktop (or RDP for short). Then copy the public IP address on the overview page and paste it next to the blank space to the right of "Computer" in Remote Desktop. Type in your username and the password then click "Connect".    
  </p>
  
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. Once you have remoted in your virtual machine, you will open up Control Panel. In Control Panel, select "Uninstall a program" under "Programs". In the pop-up, click on "Turn Windows features on or off".
</p>
<br />

<p>
<img src="https://imgur.com/kSyqpaC" height="80%" width="80%" alt="Control Panel"/>
</p>
<p>
4. Now you will want to install and enable IIS with CGI. In the Windows features pop-up window, mark the box next to "Internet Information Services" and click the plus icon to expand the options. Next, expand Application Development Features and check the box next to "CGI". 
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. Now that IIS is enabled, download and install both PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) and the Rewrite Module (rewrite_amd64_en-US.msi) from the “osTicket-Installation-Files” folder.
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. Create a new directory named "PHP" in your C drive (C:\PHP)
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. Next, you will download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the file into C:\PHP, the new directory you just created.
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. Download and install VC_redist.x86.exe from the “osTicket-Installation-Files” folder.
</p>
<br />

<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9. Next, you will install MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the “osTicket-Installation-Files” folder. In the setup wizard, select "Typical" for setup type -> select "Standard Configuration" for instance configuration -> make sure "Modify Security Settings" is checked and type in the root password. Click on "Next" and execute the process on the next page. 
</p>
<br />
