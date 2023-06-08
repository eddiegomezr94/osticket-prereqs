<p align="center">
<img src=https://i.imgur.com/CYzlgsS.png>
</p>

<div align="center">
<h1>osTicket - Prerequisites and Installation</h1>
</div>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTickets on an Azure virtual machine.

<h2> Environments and Technologies Used</h2>
 
  - Microsoft Azure 
  - Remote Desktop
  - Internet Information Services (IIS)
<h2> Operating System Used</h2> 
 
 - Windows 10 (21H2)
<h2> List of Prerequisites</h2>
  
  - Create Resource Group in Azure
  - Create Virtual Machine (VM) in Azure 
  - Login VM with Remote Desktop
  - Install/Enable Internet Information Services with CGI and Common HTTP
  - Create PHP folder in C:
  - Install PHP Manager for IIS
  - Install Rewrite Module
  - Install/Extract PHP 7.3.8 into PHP folder
  - Install Microsoft Visual C++
  - Install MySQL 5.5.62
  - Register PHP within IIS
  - Install/Extract osTicket v1.15.8 into wwwroot folder
  - Enable osTicket extensions
  - Rename ost-sampleconfig.php and assign new permissions
  - Set up remainder of osTicket system
  - Install Heidi SQL
  - Create Database
  - Delete Setup file
  - Set "read" only permission in ost-config.php

<h2> Installation Steps</h2>

<div align="center">
<h3> Create Resource Group in Azure</h3>
</div>
<img src=https://imgur.com/cpDJmAf.png>
 
 - The first step was to create a Resource Group in Azure in order for the Virtual Machine (VM) to be created.

<div align="center">
<h3> Create (VM) in Azure</h3>
</div>
<img src=https://imgur.com/ectsYRH.png>

 - The next step after creating a Resource Group was to create the VM that would be used to install the osTicket system.

<div align="center">
<h3> Login with Remote Desktop</h3>
</div>
<img src=https://imgur.com/ttqoM2s.png>

 - After creating the VM, copy and paste the public IP address to the Remote Desktop Connection app on your computer. Then proceed to log into the VM using the username and password made when creating the VM.

<div align="center">
<h3>Enable CGI in IIS</h3>
</div>
<img src=https://imgur.com/JxEkQ1W.png>

 - Once logging into the VM the next step is to enable CGI in order for PHP manager to install and work properly in the later steps. To do this open Control Panel-> Programs-> Turn Windows Features on/off-> Internet Information Services-> World Wide Web Services-> Application Development-> Check CGI. Another part of this step is to turn on Common HTTP features under World Wide Web Services. This step is done in order to install and use PHP manager for osTicket. 

<div align="center">
<h3> Install IIS Rewrite Module </h3>
</div>
<img src=https://imgur.com/3ML6shu.png>

 - 

<div align="center">
<h3>Install PHP Manager for IIS </h3>
</div>
<img src=https://imgur.com/f9zE0Qb.png>
 
 - 

<div align="center">
<h3> Create New Folder PHP in C: </h3>
</div>
<img src=https://imgur.com/okstLsI.png>

 - 
