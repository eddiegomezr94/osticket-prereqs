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
<div align="center">
<img src=https://imgur.com/3ML6shu.png>
</div>

 - After turning on specific features the next step is to download IIS Rewrite Module.

<div align="center">
<h3>Install PHP Manager for IIS </h3>
</div>
<img src=https://imgur.com/ENsukJB.png>
 
 - The next step is to install PHP manager for IIS.

<div align="center">
<h3> Create New Folder PHP in C: </h3>
</div>
<img src=https://imgur.com/okstLsI.png>

 - While the files are downloading go to C: drive in your files in order to create a new folder and name it PHP. 

<div align="center">
<h3> PHP 7.3.8 Download/Extract </h3>
</div>
<img src=https://imgur.com/Po9Z80F.png>

 - After making the PHP folder the next step is to download PHP 7.3.8 software. Once it finishes downloading extract all the files into the PHP folder created in the previous step.

<div align="center">
<h3> Install Microsoft Visual C++ </h3>
</div>
<div align="center">
<img src=https://imgur.com/EH65NuL.png>
</div>

- The next step is to install Microsoft Visual C++.

<div align="center">
<h3>Install MySQL 5.5.62 </h3>
</div>
<div align="center">
<img src="https://imgur.com/T2CS02r.png" width="400" height="300"/> 
<img src="https://imgur.com/qtXxJqZ.png" width="400" height="300"/> 
 </div>

- After installing Microsoft Visual, download and install My SQL 5.5.62, set it to Standard Configuration and create a password for your domain.

<div align="center">
<h3> Register PHP within IIS</h3>
</div>
<div align="center">
<img src="https://imgur.com/872MFRD.png" width="400" height="300"/> 
<img src="https://imgur.com/1lrII3g.png" width="400" height="300"/> 
 </div>

 - Once MySQL is set up, open IIS as an admin and register PHP. Click on PHP-> Register new PHP version-> Browes PHP file created in previous step-> Attach PHP.CGI file-> Click OK. Make sure to reload IIS-> Stop-> Start, in order to make sure PHP was registered and running.

<div align="center">
<h3> Install and open osTicket V1.15.8 </h3>
</div>
<div align="center">
<img src="https://imgur.com/koeWoFJ.png" width="400" height="300"/> 
<img src="https://imgur.com/kn9bzNf.png" width="400" height="300"/> 
 </div>

 - The next step is to download osTicket, and extract the "upload" folder to "wwwroot folder". To do this go to C:-> Inetpub-> wwwroot-> drag and drop "upload" folder (from download)-> once file is done extracting rename "upload" to osTicket. After the file is renamed, open osTicket through IIS and observe that certain extensions are not enabled.

<div align="center">
<h3>Enable Extensions in PHP </h3>
</div>
<div align="center">
<img src="https://imgur.com/Uti7wpD.png" width="400" height="300"/> 
<img src="https://imgur.com/obeurld.png" width="400" height="300"/> 
 </div>

 - After observing that some extensions are not enabled, in order to enable certain extensions go back to IIS-> Sites-> Default-> osTicket-> PHP Manager-> Enable: php_imap.dll/php_intl.dll/php_opcache.dll. After enabling extensions reload IIS, open osTicket and observe extensions enabled.


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 

<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 

<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 


<div align="center">
<h3> </h3>
</div>
<img src=.png>

 - 







