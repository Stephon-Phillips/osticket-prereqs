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
  
  <img width="80%" height="80%" alt="Screenshot (206)" src="https://github.com/user-attachments/assets/f9ab4ef4-9a14-4034-a817-5797645bc08e" />
</p>
<p>
Create a Windows 10 virtual machine in Azure and connect to it using Remote Desktop.
</p>
<br />

<h3>2. Install IIS and required IIS modules.</h3>
<p>
<img width="80%" height="80%" alt="Screenshot (210)" src="https://github.com/user-attachments/assets/e57e9907-01a8-413f-bd17-693dc2803bb2" />
</p>
<p>
Enable IIS through Windows Features and install PHP Manager and the URL Rewrite Module.
</p>
<br />

<h3>3. Install PHP and MySQL.</h3>  
<p>
<img width="80%" height="80%" alt="Screenshot 2025-11-14 145837" src="https://github.com/user-attachments/assets/7874e533-0f83-4ce5-aabc-c1ae74fded4f" />
</p>
<p>
Extract PHP into the system directory and install MySQL to store osTicket data.
</p>
<br />

<h3>4. Configure PHP with IIS.</h3>  
<p>
<img width="80%" height="80%" alt="Screenshot (211)" src="https://github.com/user-attachments/assets/2f15384d-5d75-416a-9b09-d3200f856ddd" />
</p>
<p>
Use PHP Manager to register the PHP executable and restart IIS to apply changes.
</p>
<br />

<h3>5. Unzip and place osTicket in the IIS root directory.</h3>  
<p>
<img width="80%" height="80%" alt="Screenshot (212)" src="https://github.com/user-attachments/assets/4841d94c-c2d5-4a9f-bc6f-2119935f40d5" />
</p>
<p>
Extract the osTicket files and move them into the `wwwroot` folder so IIS can serve the application.
</p>
<br />

<h3>6. Enable required PHP extensions.</h3> 
<p>
<img width="80%" height="80%" alt="Screenshot (213)" src="https://github.com/user-attachments/assets/f38e5cb3-cce0-4fd6-8732-ba6c8517ee05" />
</p>
<p>
Activate specific PHP extensions needed for email, internationalization, and caching.
</p>
<br />

<h3>7. Adjust file permissions for osTicket.</h3>  
<p>
<img width="80%" height="80%" alt="Screenshot (214)" src="https://github.com/user-attachments/assets/929cda75-05cc-48cc-a329-c435d4339ab4" />
</p>
<p>
Update the configuration file permissions to allow osTicket to write necessary settings.
</p>
<br />

<h3>8. Create the database in MySQL using HeidiSQL.</h3>  
<p>
<img width="80%" height="80%" alt="Screenshot (215)" src="https://github.com/user-attachments/assets/eae74799-d999-411a-b39c-7a9706b51780" />
</p>
<p>
Connect with root credentials and create a new database that osTicket will use.
</p>
<br />

<h3>9. Complete the osTicket web-based installer.</h3>
<p>
<img width="80%" height="80%" alt="Screenshot (216)" src="https://github.com/user-attachments/assets/214bec64-1f81-4999-90dd-6b5a96aa4bb6" />
</p>
<p>
Open the setup page in the browser and finish the installation by entering system and database details.
</p>
<br />


<h3>Finally</h3>
you'll be greeted with this page where you can find the links to either submit tickets or login as admin to see the tickets submitted.
<table>
  <tr>
    <td><img width="1920" height="1080" alt="Screenshot (217)" src="https://github.com/user-attachments/assets/719028ec-143c-4e46-96cf-e4184d72909e" /></td>
    <td><img width="1920" height="1080" alt="Screenshot (218)" src="https://github.com/user-attachments/assets/4a9f8afa-fcad-41e2-ae56-621fee9067bd" /></td>
  </tr>
  <tr>
    <td><img width="1920" height="1080" alt="Screenshot (219)" src="https://github.com/user-attachments/assets/588aa83f-20d2-48a5-9500-37eb091f6f7f" /></td>
    <td><img width="1920" height="1080" alt="Screenshot (220)" src="https://github.com/user-attachments/assets/bf6cc91b-f4ee-4067-baee-707b0efaa509" /></td>
  </tr>
</table>
