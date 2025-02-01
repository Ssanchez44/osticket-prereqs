<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### YouTube: How To Install osTicket with Prerequisites
- (https://www.youtube.com/watch?v=fWX1Lj-rOa0)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Setup a Virtual Machine in Azure
- Install the osTicket requirements
- Install osTicket itself
- configuration of osTicket
- explore osTicket as a Help Desk Professional

   
- Enable internet information service
- Install /Enable IIS in Windows WITH CGI
- Install /PHP Manager for IIS
- install the Rewrite Module 
- Intall C++ redistribuatable
- Install MySQL

<h2>Installation Steps</h2>

<p>

  
![image](https://github.com/user-attachments/assets/616048fc-06ef-4e18-b5cb-f0808d44f31a)

![image](https://github.com/user-attachments/assets/6960c180-0f0f-421f-83a9-08bd90b7a5fb)

![image](https://github.com/user-attachments/assets/c592dec9-c5af-4dce-9ade-f6083f456c68)

![image](https://github.com/user-attachments/assets/3461f189-cf05-4243-95f8-fdb7cad3ff03)


</p>

<p>
   
How to Create a Virtual Machine on Microsoft Azure
Follow these steps to create a virtual machine (VM) in Microsoft Azure:

Step 1: Access Microsoft Azure
Go to the Microsoft Azure portal or search for "Microsoft Azure" in the search bar.
Sign in to your Azure account.

Step 2: Search for Virtual Machines
In the search bar at the top, type “Virtual Machines” and select the Virtual Machines option.

Step 3: Create a Virtual Machine
Click on Create a Virtual Machine.

Step 4: Configure Resource Group
Under Resource Group, click Create new.
Name the resource group as osTicket (or any other name you prefer for your project).

Step 5: Name the Virtual Machine
Under Virtual Machine Name, enter the desired name for your VM. For this example, name it osticket-vm.

Step 6: Select Region
Under Region, choose the appropriate region closest to you. (Note: The region may vary depending on your location.)

Step 7: Select Image
Scroll down to the Image section.
From the Image dropdown, select Windows 10 Pro, version 22H2 - X64 Gen2.

Step 8: Choose VM Size
Scroll further down to the Size section.
Click Change size and select Standard_D2s_v3 (2 vCPUs, 8 GiB memory).

Step 9: Configure Authentication
Scroll to the Administrator Account section under User.
Enter a username (e.g., admin) and create a password you will remember.
Confirm the password.

Step 10: Review and Create
Review all your settings to ensure they are correct.
Once you’re satisfied, click Review + Create.
After validation, click Create.

  
   </p>

<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/3b3de1a5-a464-4bbc-9948-3a9cf599c1e0)

![image](https://github.com/user-attachments/assets/4be2daa2-6055-461a-a309-539eda4c9209)

![image](https://github.com/user-attachments/assets/646f0e09-f563-4bb5-947a-14e5dc1c63e0)



</p>
<p>
After creating your VM on Azure, follow these steps to access it using Remote Desktop.

Step 1: Get the Public IP Address of Your VM
Navigate back to the Virtual Machine you just created in the Azure portal.
Under the Overview section, locate the Public IP address.
Copy the Public IP address. This will be used to connect to your VM.

Step 2: Open Remote Desktop
On your local computer, open the Remote Desktop Connection tool. You can search for "Remote Desktop" or run mstsc in the Start menu (Windows) or use the equivalent on your system.

Step 3: Enter the IP Address
In the Remote Desktop Connection window, paste the Public IP address you copied earlier into the Computer field.

Step 4: Enter Your Username
In the Username field, enter the username you set during the VM creation process.

Step 5: Click Connect
Click Connect to begin the remote desktop session.

Step 6: Enter Your Password
enter the password you set for the username during the VM setup process.
Then Press OK.

Step 7: Access Your VM
After entering your credentials, you should successfully connect to your VM and see the Windows desktop environment of your Virtual Machine

</p>

<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

<p>

  
![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>
By checking the Internet Information Services It sets up a web server environment on your system, allowing it to host websites and web applications.</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/ef9a0bfd-b551-4386-8ee3-940bf368ac2e)

</p>
<p>
CGI (Common Gateway Interface) is a required dependency for OsTicket to function properly on the web server.</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/0864ad33-bb0e-4e62-8fd8-e23401d40000)

</p>
<p>
PHP is a server-side scripting language used for backend web development.</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/85cd0e1f-a61b-432e-b00a-41b40ad98cd9)

</p>
<p>
The Rewrite Module (mod_rewrite) is a tool that allows for URL manipulation, enabling cleaner, more user-friendly URLs and improving website functionality.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/2125d24f-d58b-4691-963e-b61f1bf0387d)

</p>
<p>
OsTicket requires VC_redist.x86.exe because it installs the necessary Visual C++ runtime components that the application depends on to function properly.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/c8e2c575-6591-4f76-8801-9f50bf7d7222)

</p>
<p>
OsTicket requires MySQL because it is the database version compatible with the software's data storage and management that needs ensuring stable performance and compatibility with the features and queries used by OsTicket.
</p>
<br />
