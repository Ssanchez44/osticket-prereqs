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

  
![image](https://github.com/user-attachments/assets/a2fdaf28-bb29-4bdd-a5af-f603cdd0901a)

![image](https://github.com/user-attachments/assets/92c7974d-06fc-4a2c-ae46-3e95fab5335d)

![image](https://github.com/user-attachments/assets/8396c049-83a8-4ea6-bba0-691c06fd21dc)

![image](https://github.com/user-attachments/assets/3da87608-82c1-4f24-813a-e73b5fb22d05)

![image](https://github.com/user-attachments/assets/a182c23f-b6fa-4a9a-ace3-10a3cf4f3965)





</p>
<p>
Step 1: Download the osTicket Installation Files
Download the file osTicket-Installation-Files.zip that I’ve provided.

Step 2: Navigate to the Downloads Folder
Once the download is complete, open File Explorer.
Go to the Downloads folder where you’ll find the osTicket-Installation-Files.zip.

Step 3: Move the File to the Desktop
Drag the osTicket-Installation-Files.zip file from the Downloads folder and drop it onto your Desktop for easier access.

Step 4: Extract the Files
Right-click on the osTicket-Installation-Files.zip file on your Desktop.
Select Extract All from the context menu.
The Extract Compressed (Zipped) Folders window will appear.
Click Next to proceed with extraction.

Step 5: Wait for the Extraction to Complete
The files will begin extracting, and you’ll see a progress bar.
Once the extraction is complete, a new folder will appear on your Desktop called osTicket files.

Step 6: Delete the Original ZIP File
You can now safely delete the original osTicket-Installation-Files.zip file from your Desktop as you no longer need it.
Be careful not to delete the extracted osTicket files folder. Only delete the original ZIP file.

</p>

<br />


<p>

<p>

![image](https://github.com/user-attachments/assets/cfacdaa4-358c-4765-b3cb-f4832f99cdb5)

![image](https://github.com/user-attachments/assets/d7559a7e-cd69-46e7-ac7f-def1d1432fad)

![image](https://github.com/user-attachments/assets/7ef29c87-10a6-46f1-9789-3c8cdfb96857)

![image](https://github.com/user-attachments/assets/4bb86b99-ed91-46cc-8074-a4af6c3fb04d)

![image](https://github.com/user-attachments/assets/07c50195-05b8-4eb7-ab20-8a9fe034ff3f)

</p>
<p>

   Step 1: Enable Internet Information Services (IIS)

Open the Control Panel by searching for it using the Windows search bar.

Navigate to Programs.

Under Programs and Features, click on Uninstall a Program.

On the left-hand side, click on Turn Windows features on or off (this will open a new window).

Scroll down and locate Internet Information Services (IIS).

Check the box next to Internet Information Services to enable it.


</p>

<br />

<p>

![image](https://github.com/user-attachments/assets/ef9a0bfd-b551-4386-8ee3-940bf368ac2e)

![image](https://github.com/user-attachments/assets/fd67b282-2a84-42ba-9a2b-a75a0189d552)


</p>
<p>

  Step 1: Open the Control Panel by searching for it using the Windows search bar.

Navigate to Programs.

Under Programs and Features, click on Uninstall a Program.

On the left-hand side, click on Turn Windows features on or off (this will open a new window).

Scroll down and locate Internet Information Services (IIS).

Check the box next to Internet Information Services to enable it.

Click OK and allow Windows to apply the changes.


Step 2: Enable CGI for osTicket

Expand Internet Information Services (IIS) by clicking the plus (+) icon.

Locate and expand World Wide Web Services.

Expand Application Development Features.

Check the box next to CGI to enable it.

Click OK to apply the changes and install the necessary web server components.

</p>

<br />

<p>

![image](https://github.com/user-attachments/assets/0864ad33-bb0e-4e62-8fd8-e23401d40000)

![image](https://github.com/user-attachments/assets/f27b55a2-c4a8-44e9-a040-4fa9e95a827e)


</p>

<p>

Step 1: Navigate to your osTicket files folder.

Locate and open the PHP Manager directory.

Run the installation file to install PHP Manager.

PHP is a server-side scripting language used for backend web development.</p>


<br />

<p>

![image](https://github.com/user-attachments/assets/85cd0e1f-a61b-432e-b00a-41b40ad98cd9)

![image](https://github.com/user-attachments/assets/fc0addb4-ff00-4bd1-a4df-c11eb3fe9f95)


</p>

<p>

 Step 1: Navigate to your osTicket files folder.

Locate and open the rewrite_amd64 directory.

Run the installation file to install URL Rewrite.

The Rewrite Module (mod_rewrite) is a tool that allows for URL manipulation, enabling cleaner, more user-friendly URLs and improving website functionality.


<br />

<p>

![image](https://github.com/user-attachments/assets/75110a13-e000-4779-be0c-523c187dec0a)

![image](https://github.com/user-attachments/assets/d93870db-9d0b-4133-b743-689c74715c1b)

![image](https://github.com/user-attachments/assets/6741cfa8-5d2c-46eb-81bd-228047f03989)

![image](https://github.com/user-attachments/assets/1c5c7886-3ac2-47f4-b326-9640080ea191)





</p>
<p>

Step 1: Open File Explorer and navigate to the *C:* drive.

Create a new folder and name it PHP.

Step 2: Extract PHP Files

Go back to the osTicket files folder.

Locate the file php7.3.8-nts.

Right-click on php7.3.8-nts and select Extract All.

When prompted to choose a destination, navigate to the C:\PHP folder created in the previous step.

Select the C:\PHP folder and click Extract.

</p>


<br />

<p>

![image](https://github.com/user-attachments/assets/2125d24f-d58b-4691-963e-b61f1bf0387d)

![image](https://github.com/user-attachments/assets/ecbf8e62-097f-4be4-96e1-f2e94dac0b87)


</p>

<p>

Navigate to your osTicket files folder.

Locate and open the VC_redist.x86 directory.

Run the installation file to install VC_redist.x86.exe

OsTicket requires VC_redist.x86.exe because it installs the necessary Visual C++ runtime components that the application depends on to function properly.

</p>


<br />


<p>

![image](https://github.com/user-attachments/assets/c8e2c575-6591-4f76-8801-9f50bf7d7222)

![image](https://github.com/user-attachments/assets/3fbbe755-f068-4023-845f-957c909cd4fd)

![image](https://github.com/user-attachments/assets/71627d54-aba6-461a-bbdd-efc9303fafec)

![image](https://github.com/user-attachments/assets/f87f7a62-d374-4192-b2b9-cc55e54b0560)

![image](https://github.com/user-attachments/assets/078bd592-f9ca-4074-b395-1c6d797669fe)

![image](https://github.com/user-attachments/assets/9311d452-6355-46f3-9c5d-35b4ddcb93ed)

![image](https://github.com/user-attachments/assets/37f18a7c-122e-4541-868f-71067a3194f2)




</p>

<p>

   Step 1: After Installing MySQL:
Select Next to continue with the MySQL setup.

Step 2: Choose Configuration Type:
When a new window pops up, select Standard Configuration.
Click Next.

Step 3: Leave the Default Settings:
On the next screen, leave all settings as they are (do not change anything).
Click Next.

Step 4: Set the MySQL Root Password:
This is a crucial step. Under the Accounts and Roles section, for the New Password and User, input root as the password.
Important: Make sure to use the password "root" exactly as specified. This will be the root user’s password.
Click Next.

Step 5: Execute Configuration:
On the next screen, click Execute.
MySQL will begin configuring itself. This may take a little time.

Step 6: Finish Setup:
Once the configuration is completed, click Finish to exit the setup.

OsTicket requires MySQL because it is the database version compatible with the software's data storage and management that needs ensuring stable performance and compatibility with the features and queries used by OsTicket.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/71e5d2f2-ac3a-4933-bb78-3e4ba701bd4b)

![image](https://github.com/user-attachments/assets/6b210147-5a63-4e58-9d82-7e1163dc7f77)

![image](https://github.com/user-attachments/assets/87c77c68-b4f3-43a9-a4ce-9bfcbac83940)

![image](https://github.com/user-attachments/assets/851d6425-b944-43ae-beba-b1aa2036a79e)

![image](https://github.com/user-attachments/assets/29fb0cd7-40e1-4a49-bd39-9c8eeb4f1ae2)

![image](https://github.com/user-attachments/assets/988791fd-c427-4bfd-a016-673e061f88bc)

![image](https://github.com/user-attachments/assets/a70e2d75-282f-4be7-baef-95f45fc29b2b)

![image](https://github.com/user-attachments/assets/044de7e0-5fd8-4ddb-ae8e-dc6679d152c0)

![image](https://github.com/user-attachments/assets/f5d1a554-7efc-4fd8-bc33-e5d6fd9ab1e3)


</p>

<p>

 Step 1: Open IIS as an Administrator:
Click the Windows button on your taskbar (or press the Windows key).
Type IIS in the search bar.
Right-click on Internet Information Services (IIS) Manager in the search results and select Run as administrator.

Step 2: Register PHP with IIS:
In the IIS Manager window, look for the "Manager" section.
Select "Register new PHP version" under the "PHP Manager" section.

Step 3: Navigate to the PHP Directory:
A file explorer window will pop up asking for the PHP directory.
Navigate to the C drive and find the PHP folder you created previously. This is the folder where you extracted or installed PHP.

Step 4: Select the PHP-CGI File:
Inside the PHP folder, locate the php-cgi.exe file.
Double-click on php-cgi.exe to select it.
After selecting php-cgi.exe, click OK.

Step 5: Open IIS Manager:

If it's not already open, press the Windows key, type IIS, and open Internet Information Services (IIS) Manager as an administrator.
Locate Your Server (osticket-vm):

On the left panel, find and click on osticket-vm (it may appear as osticket-vm (osticket-vm\lab)).
Stop the IIS Process:

In the right panel under Actions, find and click Stop.
Alternatively, you can right-click on osticket-vm in the left panel and select Stop.
Restart IIS:

Once the process has fully stopped, right-click on osticket-vm again.
Click Start to restart the IIS service.

</p>

<br />


<p>


![image](https://github.com/user-attachments/assets/0b69bdae-778b-47a3-968c-0f791322ba84)

![image](https://github.com/user-attachments/assets/c300926f-969f-4673-86b6-29a09548dc6c)

![image](https://github.com/user-attachments/assets/8e835717-b36d-4403-b08d-543b86f3eefa)

![image](https://github.com/user-attachments/assets/64736e86-0a2d-430a-b143-d8940bab969d)

![image](https://github.com/user-attachments/assets/73a23d06-6007-433a-b019-dfb205136a45)

![image](https://github.com/user-attachments/assets/e75e1807-386c-48b9-8084-dc87d7027cac)

![image](https://github.com/user-attachments/assets/bba5a261-0366-4713-b4dc-60d9e47d90e3)

</p>

<p>

Step 1: Locate the osTicket Installation Folder

Step 2: Open File Explorer and navigate to the folder where you downloaded osTicket v1.15.8.
Extract the osTicket Files

Step 3:Right-click on the osTicket v1.15.8 folder.
Click Extract All and then click Extract (no need to move the files).
Wait for the extraction process to complete.
Open the Extracted osTicket Folder

Step 4: After extraction, you will see a new osTicket folder.
Click on it, and you should see two subfolders inside.
Navigate to the IIS Web Root Directory

Step 5: Open a new File Explorer window.
Navigate to C:\inetpub\wwwroot.
Move the osTicket Upload Folder

Step 6: Go back to the extracted osTicket folder you previously opened.
Open the upload folder inside it.
Drag and drop the upload folder into C:\inetpub\wwwroot.
Rename the Upload Folder

Step 7: Once the file transfer is complete, go to C:\inetpub\wwwroot.
Find the upload folder.
Right-click on it and select Rename.
Rename it to osTicket (exactly like this, case-sensitive).


</p>

<br />

<p>


![image](https://github.com/user-attachments/assets/f1c2dd5a-c923-47d1-b525-c8f48c7eedd5)

</p>

<p>

Open IIS Manager

Press the Windows key, type IIS, and select Internet Information Services (IIS) Manager.
Right-click and choose Run as administrator.
Locate the Server (osticket-vm)

In the left panel, find and click on osticket-vm.
Stop IIS

In the right panel, under Actions, click Stop.
Wait for IIS to fully stop before proceeding.
Start IIS as Admin

Click Start in the Actions panel.


</p>

<br />

<p>


![image](https://github.com/user-attachments/assets/7d6b13a4-9a69-42c2-a1a3-b20d9ebb4f2a)

![image](https://github.com/user-attachments/assets/0cbc7213-364c-44e7-838f-c7e5a473d7d4)

![image](https://github.com/user-attachments/assets/7ab3efc4-cafa-44f2-a9b3-abe6dd5b85bf)

![image](https://github.com/user-attachments/assets/defc30fc-c0db-40eb-bfbb-cc1e321a4a6f)

![image](https://github.com/user-attachments/assets/41f1256e-8cc2-4dcd-be03-bab2e5681f09)

![image](https://github.com/user-attachments/assets/51cfda85-0ff7-4ee1-8a74-9fe3167ed4ad)

![image](https://github.com/user-attachments/assets/8c0c92bd-5d0d-4943-8d21-7202eb22c08c)

</p>

<p>

Step 1: Open osTicket Installer in a Browser
Open IIS Manager

Press the Windows key, type IIS, and select Internet Information Services (IIS) Manager.
Ensure you're running it as Administrator.
Navigate to osTicket in IIS

In the left panel, expand osticket-vm.
Expand Sites, then expand Default Web Site.
Click on osTicket.
Browse to osTicket Web Installer

In the right panel under Actions, click Browse.
This should open the osTicket web installer in your default browser.
You will see some PHP extensions unchecked, meaning they need to be enabled.

Step 2: Enable Required PHP Extensions
Go Back to IIS Manager

In IIS Manager, navigate to osticket-vm > Sites > Default Web Site > osTicket.
Open PHP Manager

Click on PHP Manager in the middle panel.
Enable the Required Extensions

Click Enable or Disable an Extension.
Find and enable the following extensions:
php_imap.dll
php_intl.dll
php_opcache.dll
Refresh the osTicket Installer Page

Go back to your browser where the osTicket web installer is open.
Refresh the page, and the previously unchecked extensions should now be enabled.

</p>

<br />


<p>


![image](https://github.com/user-attachments/assets/7d6b13a4-9a69-42c2-a1a3-b20d9ebb4f2a)

![image](https://github.com/user-attachments/assets/20574c78-30d4-467d-8a27-8903dabd8eaa)

![image](https://github.com/user-attachments/assets/14c24fe5-303b-4f4f-ac2a-1cdca6d8799a)

![image](https://github.com/user-attachments/assets/17ce00a1-531b-4857-8fc7-5d20e99b5eb1)

![image](https://github.com/user-attachments/assets/22f81a8a-9d18-4154-afc5-1f29cec1c3a4)

![image](https://github.com/user-attachments/assets/2e2f4949-459a-488b-9f34-448e16172fb4)

![image](https://github.com/user-attachments/assets/f19fe4cd-708f-4fb5-8641-a448b3177451)

![image](https://github.com/user-attachments/assets/f5ed1acb-7aee-4867-8a07-b502a84ba805)


</p>

<p>

Step 1: Rename ost-sampleconfig.php to ost-config.php
Navigate to the osTicket Directory

Open File Explorer and go to:
C:\inetpub\wwwroot\osTicket\include
Find and Rename the Configuration File

Locate the file ost-sampleconfig.php.
Right-click on it and select Rename.
Change the name to ost-config.php (exactly like this).
Press Enter to confirm the rename.

Step 2: Assign Permissions to ost-config.php
Right-Click on ost-config.php

Select Properties.
Go to the Security Tab

Click on the Security tab.
Click Advanced.
Disable Inheritance

Click Disable Inheritance.
A prompt will appear—click Remove all inherited permissions.
Add New Permissions

Click Add.
Click Select a Principal.
In the Object Name field, type Everyone.
Click OK.
Grant Full Control

Check the box for Full Control.
Click OK to apply the changes.
Apply and Close


</p>

<br />

<p>


![image](https://github.com/user-attachments/assets/f575933c-9430-4131-b350-32d756bb63fd)



</p>

<p>

Open the osTicket Web Installer

If not already open, go to your browser where the osTicket installation page is running.
Enter Helpdesk Information

Helpdesk Name: Enter your name or any name you prefer for the helpdesk.
Helpdesk Email: Enter a valid email address (this will be used for support notifications).
Configure Admin User Details

First Name & Last Name: Enter your full name.
Admin Email: Use a different email than the one entered in the helpdesk email field.
Username: Choose a username (this will be used to log in).
Password: Create a strong password and remember it (you'll need it to log in).

</p>

<br />

<p>


![image](https://github.com/user-attachments/assets/cdad13f5-6c62-4ecc-838d-bc4d87b780ef)

![image](https://github.com/user-attachments/assets/95e5be95-69dc-466b-bd39-6a6103298883)

![image](https://github.com/user-attachments/assets/f3a6ea77-f29e-414d-877e-d0384e132e4d)

![image](https://github.com/user-attachments/assets/406f60c5-6788-41ff-a03b-294f792cc228)

![image](https://github.com/user-attachments/assets/61c41b76-24bb-42ba-b4aa-d8680e5b4a7b)

![image](https://github.com/user-attachments/assets/4ec9af0b-5898-4aac-9823-5cdfc84a0191)



</p>

<p>

Step 1: Install HeidiSQL
Navigate to the osTicket Installation Files

Open File Explorer and go to the folder where you have your osTicket installation files.
Find and Install HeidiSQL

Locate the HeidiSQL installer.
Double-click it to start the installation.
Click OK and proceed with the installation.
Complete the Installation

Once the installation is done, click Finish.
A pop-up may appear—just skip it.

Step 2: Set Up a New Database Connection
Open HeidiSQL

After installation, launch HeidiSQL.
Create a New Connection

Click on New to create a new connection.
Enter Database Credentials

User: root
Password: root
Leave other settings as default.
Open the Connection

Click Open to connect to the database server.

Step 3: Create the osTicket Database
Locate the "Unnamed" Section

In the left panel, find Unnamed and right-click it.
Select Create New > Database.
Enter Database Name

Type osTicket (exactly like this, case-sensitive).
Click OK to create the database.


</p>

<br />

<p>


![image](https://github.com/user-attachments/assets/133f9357-d2c1-4d32-afbf-03891a59caa6)

![image](https://github.com/user-attachments/assets/88d20140-4d33-4481-a6ef-49af48dfc746)




</p>

<p>

Step 1: Continue osTicket Setup in the Browser
If not already open, go back to your browser where the osTicket web installer is running.
Scroll down to the MySQL Database Settings section.

Step 2: Enter MySQL Database Details
Database Name: osTicket (must match the database you created in HeidiSQL).
Username: root
Password: root
Leave other settings as default.

Step 3: Install osTicket
Double-check all the details to ensure accuracy.
Click Install Now.
Wait for the installation to complete.

Step 4: Confirmation Message
Once installed, you should see a "Congratulations" message confirming a successful installation.



</p>

<br />
