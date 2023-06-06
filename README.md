<p allign="center">
<img src=https://i.imgur.com/CYzlgsS.png>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
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

<h3> Create Resource Group in Azure</h3>

<img src=https://imgur.com/cpDJmAf.png>

  - The first step was to create a Resource Group in Azure in order for the Virtual Machine (VM) to be created.


<h3> Create (VM) in Azure</h3>
<img src=https://imgur.com/ectsYRH.png>
  
 

