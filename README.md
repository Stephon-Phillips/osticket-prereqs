<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
In this tutorial, I'll show you how to set up a Virtual Machine in Azure to install osticket, which is a free, open-source software that can be used to manage tickets and day to day task of IT staff. .<br />

<h2>Video Demonstration</h2


- ### [YouTube: How To Install osTicket using a Virtual Machine](https://youtu.be/CaoJ2CE5cn0)

<h2>Environments and Technologies Used</h2>

- Azure Windows 10 VM  
- IIS  
- PHP 7.3.8  
- MySQL 5.5.62  
- PHP Manager  
- URL Rewrite Module  
- HeidiSQL  
- osTicket v1.15.8  

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- Azure account and ability to deploy a Windows 10 VM (2 vCPUs)  
- RDP access to the VM  
- osTicket installation package  
- IIS installed with required modules  
- PHP and MySQL installers  
- Admin access to configure IIS, PHP, and MySQL  

<h2>Installation Steps</h2>
<h3>1. Deploy and access the Azure VM.</h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a Windows 10 virtual machine in Azure and connect to it using Remote Desktop.
</p>
<br />

<h3>2. Install IIS and required IIS modules.</h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable IIS through Windows Features and install PHP Manager and the URL Rewrite Module.
</p>
<br />

<h3>3. Install PHP and MySQL.</h3>  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Extract PHP into the system directory and install MySQL to store osTicket data.
</p>
<br />

<h3>4. Configure PHP with IIS.</h3>  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Use PHP Manager to register the PHP executable and restart IIS to apply changes.
</p>
<br />

<h3>5. Unzip and place osTicket in the IIS root directory.</h3>  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Extract the osTicket files and move them into the `wwwroot` folder so IIS can serve the application.
</p>
<br />

<h3>6. Enable required PHP extensions.</h3> 
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Activate specific PHP extensions needed for email, internationalization, and caching.
</p>
<br />

<h3>7. Adjust file permissions for osTicket.</h3>  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Update the configuration file permissions to allow osTicket to write necessary settings.
</p>
<br />

<h3>8. Create the database in MySQL using HeidiSQL.</h3>  
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Connect with root credentials and create a new database that osTicket will use.
</p>
<br />

<h3>9. Complete the osTicket web-based installer.</h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the setup page in the browser and finish the installation by entering system and database details.
</p>
<br />
