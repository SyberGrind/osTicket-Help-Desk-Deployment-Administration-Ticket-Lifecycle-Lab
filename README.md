# osTicket-Lab

# Define the content for the README.md
readme_content = """# osTicket Deployment and Configuration Lab

This repository documents the end-to-end deployment, configuration, and management of an **osTicket** help desk system hosted on an Azure Virtual Machine.

## Documentation Overview
The following steps outline the complete lifecycle of the lab, from infrastructure provisioning to ticket resolution workflows.

---

### Phase 1. Azure Infrastructure & VM Setup

* **Step 1:** Accessing the Azure Resource Group portal.
* <img width="1366" height="768" alt="Step 1  Launch of Resource Group Portal" src="https://github.com/user-attachments/assets/b1814483-62d5-4e5d-995c-3e511ae4fcd7" />

* **Step 2:** Configuring Resource Group name "Tickets" and selecting the East Asia region.
* <img width="1366" height="768" alt="Step 2  Naming the reasource group Tickets   Selecting Zone East Asia" src="https://github.com/user-attachments/assets/ac9dbd3c-7003-4c31-aa9b-3f67fed2c207" />

* **Step 3:** Initiating Resource Group creation.
* <img width="1366" height="768" alt="Step 3  Creating Resource Group" src="https://github.com/user-attachments/assets/0f17410e-642c-44c7-8db5-b9bd806f4cd5" />

* **Step 4:** Resource Group successfully provisioned.
* <img width="1366" height="768" alt="Step 4  Successfull Creation of Reasouce Group" src="https://github.com/user-attachments/assets/74deafc4-10bc-4c1f-8cf3-fd3b3df08480" />


* **Step 5:** Navigating to the Virtual Machine creation portal.
* <img width="1366" height="768" alt="Step 5  Initialization of Virtual Machine Portal" src="https://github.com/user-attachments/assets/16276143-1d33-4d81-9b5c-0880a659ed07" />

* **Step 6:** Virtual Machine deployment wizard initialized.
* <img width="1366" height="768" alt="Step 6  Virtual Machine Creation Portal successfully launched" src="https://github.com/user-attachments/assets/69413075-aaf0-4983-ba3b-43d220dd37b2" />

* **Step 7:** Selecting Windows 11 Pro image and appropriate instance size.
* <img width="1366" height="768" alt="Step 7  Virtual Machine Creation Portal  Seleted Windows 11 Pro as iamge   size" src="https://github.com/user-attachments/assets/ec78d081-3b9d-40fb-a37d-42ea93856298" />

* **Step 8:** Proceeding through VM configuration settings.
* <img width="1366" height="768" alt="Step 8  Virtual Machine Creation Porta" src="https://github.com/user-attachments/assets/2342c060-7a10-4f17-abce-f3c5ec74906a" />

* **Step 9:** Setting deployment scope: Resource Group "Tickets", VM name "osTicketVM", and East Asia region.
* <img width="1366" height="768" alt="Step 9  Virtual Machine Creation Portal - Adding Credentials Resource Group Tickets, Name osTicketVM   Zone East Asia" src="https://github.com/user-attachments/assets/829a2573-9212-4714-9d4b-822d0071fd6b" />

* **Step 10:** Defining administrative credentials and security settings for `osTicketVM`.
* <img width="984" height="1600" alt="Step 10  Credentilas such as password   name for osTicketVM" src="https://github.com/user-attachments/assets/d029d83b-9985-4495-92a2-477a2d488bfb" />

* **Step 11:** Finalizing VM deployment parameters.
* <img width="1366" height="768" alt="Step 11  Adding final credentilas for Tickets VM creation" src="https://github.com/user-attachments/assets/98ec3b83-6d80-4353-965b-3c89e3e96dd2" />

* **Step 12:** Reviewing and confirming deployment for `osTicketVM`.
* <img width="1366" height="768" alt="Step 12  Confirming Creation of Tickets VM" src="https://github.com/user-attachments/assets/cc5dc99d-0dac-4d1d-9805-e42f06a9731b" />

* **Step 13:** Virtual Machine deployment successfully completed.
* <img width="1366" height="768" alt="Step 13  Successful Creation of osTicketVM" src="https://github.com/user-attachments/assets/9d965b7c-8555-4d20-bcd6-5f6de780da7f" />

* **Step 14:** Retrieving the Public IP address for Remote Desktop Connection.
* <img width="1366" height="768" alt="Step 14  Copying public IP Address of osTicketVM on Remote Desktop Connection" src="https://github.com/user-attachments/assets/686fd7c1-691a-4d7f-b3c3-19de6e1fa19d" />

* **Step 15:** Establishing RDP connection with IP `40.81.28.195` and username "Tickets".
* <img width="1366" height="768" alt="Step 15  Adding credentials Public IP address 40 81 28 195   name Tickets to launch osTicketVM" src="https://github.com/user-attachments/assets/261dba99-2d52-4a92-ad47-8b0c029c4b12" />

* **Step 16:** Authenticating RDP session with administrative password.
* <img width="1366" height="768" alt="Step 16  Adding last credential password to launch osTicketVM" src="https://github.com/user-attachments/assets/55b1fffd-3577-497c-b29f-cd39b301318b" />

* **Step 17:** Remote Desktop session successfully established.
* <img width="1366" height="768" alt="Step 17  Successful launch of osTicketVM" src="https://github.com/user-attachments/assets/1ab828e6-1f60-4369-9284-c66bb3ea2962" />

* **Step 18:** Verifying active RDP session via Windows interface.
<img width="1366" height="768" alt="Step 18  Confirming I am in osTicketVM again by clicking windows key" src="https://github.com/user-attachments/assets/b587a0ed-b734-45df-817b-ac4a5a372f13" />

### Phase 2. Software Download & IIS Configuration

* **Step 19:** Opening Microsoft Edge to download the osTicket source files.
<img width="1366" height="768" alt="Step 19  Opening Microsoft Edge to download osTicket Installation file" src="https://github.com/user-attachments/assets/059f8668-66c1-435e-a542-5acdd17f8815" />

* **Step 20:** Accessing the osTicket download page.
* <img width="1366" height="768" alt="Step 20  Successful lauch of page to download osTicket installation file" src="https://github.com/user-attachments/assets/e4a6daf9-616a-44f5-b207-b1fddb01d26a" />

* **Step 21:** osTicket installation package successfully downloaded.
* <img width="1366" height="768" alt="Step 21  Successful downlaod of osTicket installation file to download folder" src="https://github.com/user-attachments/assets/3c425a1e-3b54-4ac7-b130-bdc8b8650508" />

* **Step 22:** Moving the installation package to the Desktop for easier access.
* <img width="1366" height="768" alt="Step 22  Moved osTicket installation file to Desktop folder" src="https://github.com/user-attachments/assets/97df4693-0b6e-4e81-ae12-223fd888d245" />

* **Step 23:** Verifying installation file location on the Desktop.
* <img width="1366" height="768" alt="Step 23  Confirmation osTicket installation file is in the Desktop folder page" src="https://github.com/user-attachments/assets/6acfa64c-428e-4cba-a4e0-0110823da746" />

* **Step 24:** Initializing extraction of the osTicket archive.
* <img width="1366" height="768" alt="Step 24  Extracting osTicket installation files" src="https://github.com/user-attachments/assets/fce2ca08-b22b-4114-848c-2edd07c7f22c" />


* **Step 25:** Defining target path for extraction to the Desktop.
* <img width="1366" height="768" alt="Step 25  Extracting the files to desktop" src="https://github.com/user-attachments/assets/be914c0e-21a7-4f3a-abe4-031644ddeebc" />

* **Step 26:** Extraction process completed successfully.
* <img width="1366" height="768" alt="Step 26  Successfull extraction of files" src="https://github.com/user-attachments/assets/e2c6407a-24c7-4869-97b3-468ef9ef12bf" />

* **Step 27:** Accessing the Windows Control Panel via the search bar.
* <img width="1366" height="768" alt="Step 27  Went to the search bar to look for Control Panel to launch it" src="https://github.com/user-attachments/assets/2135f233-7715-4080-bb85-92b19ffd9e6e" />

* **Step 28:** Control Panel interface launched.
* <img width="1366" height="768" alt="Step 28  Successful lauch of Control Panel" src="https://github.com/user-attachments/assets/a6a7c898-461b-4290-a45b-651eb1173508" />

* **Step 29:** Navigating to the "Programs and Features" management console.
* <img width="1366" height="768" alt="Step 29  Navigated to Programs on Control Panel to Launch it" src="https://github.com/user-attachments/assets/a89216f3-87ae-442e-811a-1cbfe7d7d3f3" />

* **Step 30:** Programs console opened successfully.
* <img width="1366" height="768" alt="Step 30  Successful launch of Programs on Control Panel" src="https://github.com/user-attachments/assets/bda684c3-d1da-4155-b339-9686bdb893b5" />

* **Step 31:** Accessing "Turn Windows features on or off" to configure IIS.
* <img width="1366" height="768" alt="Step 31  Launched Windows features to set up CGI" src="https://github.com/user-attachments/assets/f1ed8114-bc29-4f49-8b62-1b0b109d0183" />

* **Step 32:** Locating Internet Information Services in the features list.
* <img width="1366" height="768" alt="Step 32  Scrolled to down Internet Information Services to open it on Windows Features" src="https://github.com/user-attachments/assets/7097e0e6-7a93-4b1b-86ae-ec4844b24ae5" />

* **Step 33:** Expanding IIS to access Application Development Features.
* <img width="1366" height="768" alt="Step 33  Expanded the Internet Information Services folder to navigate to Application Developement Features" src="https://github.com/user-attachments/assets/b98f1e5c-3d59-4771-9e1f-7c7503c3eeb0" />

* **Step 34:** Navigating to the CGI sub-feature.
* <img width="1366" height="768" alt="Step 34  Expanded Application Developement Features to locate CGI" src="https://github.com/user-attachments/assets/2ef8d23b-1fcb-40fa-a80c-397b9dcc1ead" />

* **Step 35:** Enabling and installing the CGI module.
* <img width="1366" height="768" alt="Step 35  Clicked on CGI to download it on Windows Features within the Application Development Features" src="https://github.com/user-attachments/assets/85171e09-58a3-4938-bb09-ceab86ae2b44" />

* **Step 36:** CGI module installation confirmed.
* <img width="1366" height="768" alt="Step 36  Successful download of CGI" src="https://github.com/user-attachments/assets/969c01c3-b1bf-4593-ac71-f260cf0a8cb4" />

* **Step 37:** Launching Microsoft Edge to verify the IIS web server.
* <img width="1366" height="768" alt="Step 37  Launch of  Microsoft Edge to intiate IIS - Internet Information Services" src="https://github.com/user-attachments/assets/11aad997-f197-4242-97e2-155f52d71a94" />

* **Step 38:** Verifying IIS functionality by accessing the local loopback address `127.0.0.1`.
<img width="1366" height="768" alt="Step 38  Prompted loop back address 127 0 0 1 to Successfully launch IIS - Internet Information Services" src="https://github.com/user-attachments/assets/778320da-7375-4132-aeab-0ef38ab3425c" />

### Phase 3. PHP & Database Setup
* **Step 39:** Accessing the installation directory to run the PHP installer.
* <img width="1366" height="768" alt="Step 39  Navigated back to osTicket Installation Files to install PHP" src="https://github.com/user-attachments/assets/c50674a2-7e73-421f-8cf8-c98c8953d60d" />

* **Step 40:** Locating the PHP executable for installation.
* <img width="1366" height="768" alt="Step 40  Opened the installation file to locate PHP for installation" src="https://github.com/user-attachments/assets/37f95c80-86d4-432d-97f6-cbcdf69897a0" />

* **Step 41:** Running the PHP setup wizard.
* <img width="1366" height="768" alt="Step 41  Setting up PHP to install it" src="https://github.com/user-attachments/assets/765cb693-bf34-4b02-9b9b-5196933fa8ba" />

* **Step 42:** PHP installed successfully.
* <img width="1366" height="768" alt="Step 42  Successful installation of PHP" src="https://github.com/user-attachments/assets/7a39abb0-9a60-4f64-8d7c-14a76aef6691" />

* **Step 43:** Accessing the installation directory to run the URL Rewrite Module installer.
* <img width="1366" height="768" alt="Step 43  Navigated back to osTicket Installation Files to Launch  REWRITE MODULE  to Install it" src="https://github.com/user-attachments/assets/6697eb5e-0cb2-4c8c-bb27-e23c41f08815" />

* **Step 44:** Running the URL Rewrite Module setup wizard.
* <img width="1366" height="768" alt="Step 44  REWRITE Module Setup for Installation" src="https://github.com/user-attachments/assets/52f4e301-47e4-4242-9926-a8700d3cae9b" />

* **Step 45:** URL Rewrite Module installed successfully.
* <img width="1366" height="768" alt="Step 45  Successfull Installation of REWRITE MODULE" src="https://github.com/user-attachments/assets/50a5c791-7275-40cd-b1ed-5e9149db3456" />

* **Step 46:** Accessing the C: drive to prepare the PHP directory.
* <img width="1366" height="768" alt="Step 46  Navigating to my Windows C drive to create PHP folder" src="https://github.com/user-attachments/assets/e254d51a-14e5-44f1-842e-f1b714026b6a" />

* **Step 47:** Creating the `C:\PHP` directory.
* <img width="1366" height="768" alt="Step 47  Creating a folder of PHP in Windows C drive" src="https://github.com/user-attachments/assets/8831f893-4380-4e3c-95ca-263667fab2ac" />

* **Step 48:** PHP directory created successfully.
* <img width="1366" height="768" alt="Step 48  Successful creation of PHP folder" src="https://github.com/user-attachments/assets/c6b8b9bc-0173-4064-a24b-20b0360b66b5" />

* **Step 49:** Initiating the copy of PHP binaries to the `C:\PHP` directory.
* <img width="1366" height="768" alt="Step 49  Opening osTicket Installation File to extract PHP 738 files to PHP folder in Windows C drive" src="https://github.com/user-attachments/assets/d918c245-fe39-4afd-a073-122948137bd0" />

* **Step 50:** Extracting PHP binaries to `C:\PHP`.
* <img width="1366" height="768" alt="Step 50  Extracting PHP 738 files to PHP folder in Windows C drive" src="https://github.com/user-attachments/assets/f654cecf-c002-49ba-a4b1-7f0e465467ba" />

* **Step 51:** PHP binaries extraction complete.
* <img width="1366" height="768" alt="Step 51  Successful extraction PHP 738 files to PHP folder in Windows C drive" src="https://github.com/user-attachments/assets/99c695a5-dfbc-4c54-b425-af0585b4634d" />

* **Step 52:** Verifying PHP binary files in the `C:\PHP` directory.
* <img width="1366" height="768" alt="Step 52  Confirmation PHP 738 files are in PHP folder in Windows C drive" src="https://github.com/user-attachments/assets/69d5ab03-8bc7-4be7-b873-f1c990f53c81" />

* **Step 53:** Running the Microsoft Visual C++ Redistributable installer.
* <img width="1366" height="768" alt="Step 53  Navigation back to osTicket Installation File to install Microsoft Visual C" src="https://github.com/user-attachments/assets/83ee7e03-bf10-49e6-8851-8dcca3274914" />

* **Step 54:** Executing the Visual C++ installation wizard.
* <img width="1366" height="768" alt="Step 54  Installation of Microsoft Visual C" src="https://github.com/user-attachments/assets/5ca12ffc-78e7-4d47-9780-462b061cec2d" />

* **Step 55:** Visual C++ installation confirmed.
* <img width="1366" height="768" alt="Step 55  Successful Installation of Microsoft Visual C" src="https://github.com/user-attachments/assets/d0680b8d-abc2-4a3f-8544-c69dcbeec754" />

* **Step 56:** Launching the MySQL installation wizard.
* <img width="1366" height="768" alt="Step 56  Navigation back to osTicket Installation File to Install MYSQL" src="https://github.com/user-attachments/assets/dffe5ab6-62b8-4b0c-909a-e1ca54a19edc" />

* **Step 57:** Initiating MySQL setup.
* <img width="1366" height="768" alt="Step 57   Installing  MYSQL" src="https://github.com/user-attachments/assets/3f7ef130-9e78-4e3b-93f0-4a0bfb105785" />

* **Step 58:** Proceeding through MySQL configuration steps.
* <img width="1366" height="768" alt="Step 58  Installing MYSQL" src="https://github.com/user-attachments/assets/a6a13244-a3fb-47bb-9e86-5c637909fbb1" />

* **Step 59:** Configuring MySQL database settings.
<img width="1366" height="768" alt="Step 59  Installing MYSQL" src="https://github.com/user-attachments/assets/0cb41f92-e8e7-48ee-aead-840541b42f34" />

* **Step 60:** Setting the administrative password for the MySQL root account.
* <img width="1366" height="768" alt="Step 60  Defining MYSQL password to Install MYSQL" src="https://github.com/user-attachments/assets/ccc1bcaf-4c8f-46a6-a52b-91b85812c5a5" />

* **Step 61:** Accessing Internet Information Services (IIS) Manager.
* <img width="1366" height="768" alt="Step 61  Navigating to the search bar launch to ISS" src="https://github.com/user-attachments/assets/22f92b47-3588-41c2-ae4e-a5b667a7c6c6" />

* **Step 62:** Launching PHP Manager within IIS.
* <img width="1366" height="768" alt="Step 62  Successful launch of IIS - Navigating to within ISS to launch PHP Manager" src="https://github.com/user-attachments/assets/b358045a-3496-4a9a-8170-b1415300a0dd" />

* **Step 63:** PHP Manager successfully loaded.
* <img width="1366" height="768" alt="Step 63  PHP manager launched" src="https://github.com/user-attachments/assets/eb5738c1-daa5-4c36-8b67-7e474f4cfe6c" />

* **Step 64:** Linking PHP Manager to the PHP binary path.
* <img width="1366" height="768" alt="Step 64  Configuring PHP Manager by using PHP files within PHP Folder" src="https://github.com/user-attachments/assets/795e451d-14f8-4606-a177-8ea2adc8905b" />

* **Step 65:** Configuring PHP Manager to use the PHP-CGI executable.
* <img width="1366" height="768" alt="Step 65  Configuring PHP Manager by using PHP files within PHP Folder Selecting PHP CGI" src="https://github.com/user-attachments/assets/a72d3ac9-4eb3-4ec6-bd50-2e6d3bacd8de" />

* **Step 66:** Confirming PHP-CGI configuration settings.
* <img width="1366" height="768" alt="Step 66  Configuring PHP Manager by using PHP files within PHP Folder Selecting PHP CGI" src="https://github.com/user-attachments/assets/8e60ba59-2a90-495b-85f4-092c60c8b09e" />

* **Step 67:** Prompting an IIS service restart to apply PHP configurations.
* <img width="1366" height="768" alt="Step 67  Prompt to Restart IIS to update PHP Manager Settings" src="https://github.com/user-attachments/assets/6a569ee4-c607-4904-96a3-09c6d3263913" />

* **Step 68:** IIS restart completed successfully.
<img width="1366" height="768" alt="Step 68  Successful Restart of IIS to update PHP Manager Settings" src="https://github.com/user-attachments/assets/7a2c5fea-5ada-4097-bf2d-cd124d24f85a" />

### Phase 4. osTicket Deployment & Initial Configuration

* **Step 69:** Accessing the osTicket source files for final deployment.
* <img width="1366" height="768" alt="Step 69  Navigating to osTicket Installation to extract osTicket v1 15 8 files within osTicket v1 15 8" src="https://github.com/user-attachments/assets/dfb257e6-19d0-43c1-bc11-cf202ab085c6" />

* **Step 70:** Locating the `v1.15.8` directory.
* <img width="1366" height="768" alt="Step 70  Successful launch of osTicket Installation to extract osTicket v1 15 8 files within osTicket v1 15 8" src="https://github.com/user-attachments/assets/f40447e5-ceff-4adf-93eb-3c86371aa3cf" />

* **Step 71:** Extracting osTicket application files.
* <img width="1366" height="768" alt="Step 71  Extracting osTicket v1 15 8 files within osTicket v1 15 8 folder" src="https://github.com/user-attachments/assets/c57642ca-33ef-4a1d-9c7b-981f575e0086" />

* **Step 72:** Extracting source code to the project directory.
* <img width="1366" height="768" alt="Step 72  Extracting osTicket v1 15 8 files within osTicket v1 15 8 folder process" src="https://github.com/user-attachments/assets/cd7ed8c5-88a6-4d59-94e6-787a1f11d636" />

* **Step 73:** Extraction completed successfully.
* <img width="1366" height="768" alt="Step 73  Successful extraction osTicket v1 15 8 files" src="https://github.com/user-attachments/assets/b417f743-00b4-45ad-92e7-b49bc8f0e22a" />

* **Step 74:** Accessing the upload directory in the osTicket source files.
* <img width="1366" height="768" alt="Step 74  Successful launch of osTicket v1 15 8 folder to copy upload file" src="https://github.com/user-attachments/assets/fef89e61-45cd-416f-ac57-e9c477919cb7" />

* **Step 75:** Copying the contents of the upload folder.
* <img width="1366" height="768" alt="Step 75  Copying upload file" src="https://github.com/user-attachments/assets/7fd57588-0ebe-4a2b-9d08-52521d0af4a6" />

* **Step 76:** Deploying application files to `C:\inetpub\wwwroot\`.
* <img width="1366" height="768" alt="Step 76  Paste of upload file to wwwroot folder Within C Drive" src="https://github.com/user-attachments/assets/e8c5ae33-0ff0-42fb-8fd2-a0437a4a15c1" />

* **Step 77:** Renaming the directory to "osTicket" for easier web access.
* <img width="1366" height="768" alt="Step 77  Renaming upload file to osTicket in wwwroot within Windows C drive" src="https://github.com/user-attachments/assets/b1dfe4de-d67f-4f94-abee-cc6fd73f060b" />

* **Step 78:** Restarting IIS to register the new application.
* <img width="1366" height="768" alt="Step 78  Launch of IIS to restart it to update settings" src="https://github.com/user-attachments/assets/b84a4e76-a4f7-4935-a3fe-1cf62be7b340" />

* **Step 79:** IIS services successfully restarted.
* <img width="1366" height="768" alt="Step 79  Successful Restart of ISS" src="https://github.com/user-attachments/assets/1cb6eb6c-b843-4d98-9651-978ea3d76890" />

* **Step 80:** Verifying the Application Pool settings for the site.
* <img width="1366" height="768" alt="Step 80  Navigating to Application Pools in IIS" src="https://github.com/user-attachments/assets/33162206-7a56-4585-91d5-15305711fa4d" />

* **Step 81:** Reviewing site bindings in IIS.
* <img width="1366" height="768" alt="Step 81  Navigating to Sites in IIS" src="https://github.com/user-attachments/assets/f7e05e15-961b-425f-b1b9-51db44735e4e" />

* **Step 82:** Launching the default web site to initiate the osTicket web-based installer.
* <img width="1366" height="768" alt="Step 82  Navigating to Default Web Site to launch SEMI installed osTicket" src="https://github.com/user-attachments/assets/8227b9b1-c20b-4c83-933b-d77837e37e71" />

* **Step 83:** osTicket installer landing page displayed.
* <img width="1366" height="768" alt="Step 83  Successful launch of SEMI installed osTicket" src="https://github.com/user-attachments/assets/4efb0e0e-13d7-4f41-bfe1-05c4c04418d3" />

* **Step 84:** Navigating to the osTicket directory in IIS to manage PHP extensions.
* <img width="1366" height="768" alt="Step 84  Navigating to osTicket folder within ISS for authetication in PHP Manager" src="https://github.com/user-attachments/assets/662a00b2-f1a2-4180-a046-879cdb490f68" />

* **Step 85:** Launching Authentication management.
* <img width="1366" height="768" alt="Step 85  Prompt to launch Authetication in PHP manager" src="https://github.com/user-attachments/assets/2837d722-56c4-4d64-a2a3-487ed43d14fe" />

* **Step 86:** Accessing PHP extension management.
* <img width="1366" height="768" alt="Step 86   Successful launch of Authetication in PHP manager to start process of to enable some PHP extentions" src="https://github.com/user-attachments/assets/a10156ed-1a9b-4728-96e9-41198c4661f7" />

* **Step 87:** Viewing available PHP extensions.
* <img width="1366" height="768" alt="Step 87  Prompt to launch of PHP Extention to enable PHP extentions" src="https://github.com/user-attachments/assets/7bf3474f-40b2-4274-8104-4dc059d4e69d" />

* **Step 88:** Initiating configuration of required extensions.
* <img width="1366" height="768" alt="Step 88  Launch of PHP Extention to enable PHP extentions" src="https://github.com/user-attachments/assets/8100f860-26bf-4076-95e0-278966791abc" />

* **Step 89:** Enabling the `php_intl.dll` extension.
* <img width="1366" height="768" alt="Step 89  Enabling PHP dil withing PHP Extentions" src="https://github.com/user-attachments/assets/bb2f3c11-0540-4e21-a578-2aaeca7a7aa2" />

* **Step 90:** Enabling the `php_opcache.dll` extension.
* <img width="1366" height="768" alt="Step 90  Enabling php opcache dill within PHP Extentions" src="https://github.com/user-attachments/assets/6ac71d2f-2c27-4d8d-bedb-8413ed6631b5" />

* **Step 91:** Refreshing the osTicket installation page.
* <img width="1366" height="768" alt="Step 91  Navigated back SEM installed osTicket" src="https://github.com/user-attachments/assets/1c27f8c3-544f-467e-8790-c5015932e775" />

* **Step 92:** Modifying file permissions for `ost-sampleconfig.php` to allow renaming/writing.
* <img width="1366" height="768" alt="Step 92  Navigation to ost sampleconfig php to alter its properties in the osTicket Folder within Windows C drive" src="https://github.com/user-attachments/assets/26e30bff-0cdb-4e19-a89d-e69d566d5a4f" />

* **Step 93:** Updating security properties to grant "Everyone" modify access.
* <img width="1366" height="768" alt="Step 93  ost sampleconfig php security properties altered to everyone" src="https://github.com/user-attachments/assets/a2eeebba-5274-40a3-a1ad-040332d681a2" />

* **Step 94:** Configuring primary osTicket installation settings (Page 1).
* <img width="1366" height="768" alt="Step 94  1st Blank Credentials page of osTicket to complete intallation" src="https://github.com/user-attachments/assets/8cfdc618-744d-40b5-8452-12f32b0569ea" />

* **Step 95:** Configuring database and admin account credentials (Page 2).
* <img width="1366" height="768" alt="Step 95  2nd Blank Credentials page of osTicket to complete intallation" src="https://github.com/user-attachments/assets/4f8bd677-8a73-4f42-8ca4-19e8ccc765b0" />

* **Step 96:** Verifying final installation configurations (Page 3).
* <img width="1366" height="768" alt="Step 96  3rd Blank Credentials page of osTicket to complete intallation" src="https://github.com/user-attachments/assets/2f05896e-b6c8-4eb4-8054-c9a7644d3a4a" />

* **Step 97:** Reviewing compiled configuration credentials.
* <img width="1047" height="1600" alt="Step 97  Credentials sheet for osTicket installation" src="https://github.com/user-attachments/assets/24d0e66a-adbe-4853-b5a5-16e583112035" />

* **Step 98:** Inputting system and email settings.
* <img width="1366" height="768" alt="Step 98  Defining credentials for 1st page to intall osTicket" src="https://github.com/user-attachments/assets/87190d88-6566-4e1e-a76b-038bc31dbbfe" />

* **Step 99:** Inputting database host, name, and user credentials.
* <img width="1366" height="768" alt="Step 99  Defining credentials for 2nd page to intall osTicket" src="https://github.com/user-attachments/assets/2ba40533-5624-4edd-9c5b-4e046c769a63" />

* **Step 100:** Confirming admin account details.
* <img width="1366" height="768" alt="Step 100  Defining credentials for 3rd page to intall osTicket" src="https://github.com/user-attachments/assets/0bc7bff9-4bf3-42fe-bdbb-f7f15b8d749f" />

* **Step 101:** osTicket installation completed successfully.
* <img width="1366" height="768" alt="Step 101  Successful complete installation of osTicket" src="https://github.com/user-attachments/assets/b0fb2c7d-1617-4705-a7a8-ade41677a482" />

* **Step 102:** Inputting administrative credentials to access the portal.
* <img width="1366" height="768" alt="Step 102  Adding credentials to log in osTicket application" src="https://github.com/user-attachments/assets/94457eb4-a17c-4dfa-9fb9-7e90b889bff4" />

* **Step 103:** Successful login to the osTicket Admin Panel.
<img width="1366" height="768" alt="Step 103  Successful login to osTicket" src="https://github.com/user-attachments/assets/98ecbead-6c70-4443-9f8d-dae61183cff0" />

### Phase 5. User Management & Testing

* **Step 104:** Navigating to the Admin Panel to manage Roles.
* <img width="1366" height="768" alt="Step 104  Navigated to admin panel to start process of adding a role" src="https://github.com/user-attachments/assets/d8766949-adcd-47bc-acaf-ea6a7006c332" />

* **Step 105:** Accessing the Role management portal.
* <img width="1366" height="768" alt="Step 105  Navigated to role portal to view existing roles and to add new role" src="https://github.com/user-attachments/assets/ebe412d5-d0c0-4711-b47e-fc3c5aa4dfd6" />

* **Step 106:** Creating a new custom role: "Supreme Admin".
* <img width="1366" height="768" alt="Step 106  Naming name role Supreme Admin" src="https://github.com/user-attachments/assets/4dc965ef-99b5-4911-a3f7-07ac617fe5e5" />

* **Step 107:** Configuring ticket permissions for "Supreme Admin".
* <img width="1366" height="768" alt="Step 107  Viewing current permissions for tickets of Supreme Admin Role" src="https://github.com/user-attachments/assets/3fda39a9-d059-4bf0-aea0-f77157ca956d" />

* **Step 108:** Defining granular access levels for ticket management.
* <img width="1366" height="768" alt="Step 109  Viewing  permissions for tasks of Supreme Admin Role" src="https://github.com/user-attachments/assets/0a0c2c65-9d96-4506-a1f5-22cd00dee03a" />

* **Step 109:** Configuring task management permissions.
* <img width="1366" height="768" alt="Step 110  Viewing  permissions for knowledgebase of Supreme Admin Role" src="https://github.com/user-attachments/assets/d3dbc389-1c2b-4fc8-868d-e9ed65461a53" />

* **Step 110:** Setting Knowledgebase access permissions.
* <img width="1366" height="768" alt="Step 111  Supreme Role Added Successfully" src="https://github.com/user-attachments/assets/7d20f883-4d80-41a3-b465-8b9d5518595d" />

* **Step 111:** "Supreme Admin" role successfully created.
* <img width="1366" height="768" alt="Step 112  Adding a department in osTicket" src="https://github.com/user-attachments/assets/1f7da84a-979f-4fb6-84f1-057f89cc907c" />

* **Step 112:** Navigating to Department management.
* <img width="1366" height="768" alt="Step 112  Adding a department in osTicket" src="https://github.com/user-attachments/assets/a4401a34-cdf6-4451-9cf7-07b347f00efa" />

* **Step 113:** Defining attributes for the new "SysAdmins" department.
* <img width="1366" height="768" alt="Step 113  Define Credentials of new department" src="https://github.com/user-attachments/assets/756a13b5-7e44-4f89-b470-188c02511536" />

* **Step 114:** "SysAdmins" department created successfully.
* <img width="1366" height="768" alt="Step 114  SysAdmins Department Successfully Created" src="https://github.com/user-attachments/assets/da26ec14-cef9-4a20-b4de-0bd9ac9c8cac" />

* **Step 115:** Accessing Team management.
* <img width="1366" height="768" alt="Step 115  Creating a team on osTicket" src="https://github.com/user-attachments/assets/0de4dad8-ae85-41bc-a2c6-d348b29a49f8" />

* **Step 116:** Defining new team credentials.
* <img width="1366" height="768" alt="Step 116  Defining credentials of team being created" src="https://github.com/user-attachments/assets/6bc54c35-2737-4e9a-9dd6-3cf5912b1992" />

* **Step 117:** "SysAdmins" team created successfully.
* <img width="1366" height="768" alt="Step 117  SysAdmins Team Successfully created" src="https://github.com/user-attachments/assets/472d30d8-0429-4943-b792-9a4954e8835e" />

* **Step 118:** Accessing the Agent Directory.
* <img width="1366" height="768" alt="Step 118  Viewing existing agents" src="https://github.com/user-attachments/assets/ae9b1343-4865-48e6-ba40-0dacb774d22a" />

* **Step 119:** Initiating the creation of a new agent: "Muneni Sigana".
* <img width="1366" height="768" alt="Step 119  Adding new agent Muneni Sigana" src="https://github.com/user-attachments/assets/f189dfe5-9ae4-4f91-8eb5-c2edd8933ab6" />

* **Step 120:** Assigning the "Supreme Admin" role and "SysAdmins" department to Muneni.
* <img width="1366" height="768" alt="Step 120  Giving Muneni Supreme Admin Role   Adding them to the SysAdmin Department" src="https://github.com/user-attachments/assets/80d426ab-2bb5-4b6b-af14-4c3b62fd9181" />

* **Step 121:** Granting full administrative permissions to Muneni.
* <img width="1366" height="768" alt="Step 121  Giving Muneni all permissions" src="https://github.com/user-attachments/assets/92ab72a5-125e-4cf3-915b-98a74ea9e0dc" />

* **Step 122:** Assigning Muneni to the "Online Sales" team.
* <img width="1366" height="768" alt="Step 122  Adding Muneni to Online Sales Team" src="https://github.com/user-attachments/assets/e15010a0-6886-4152-b01d-cce132ac81a9" />

* **Step 123:** Agent "Muneni Sigana" account successfully provisioned.
* <img width="1366" height="768" alt="Step 123  Agent Muneni Sigana Successfully created" src="https://github.com/user-attachments/assets/e43dfaa0-33a9-44ff-a8fe-b3803c9ccb5e" />

* **Step 124:** Reviewing the updated Agent Directory.
* <img width="1366" height="768" alt="Step 124  Viewing list of agents" src="https://github.com/user-attachments/assets/50f49f99-1eb0-4b15-9226-6c3cfdc03061" />

* **Step 125:** Initiating the creation of a new agent: "Tshidi Bosiu Thaba".
* <img width="1366" height="768" alt="Step 125  Creating Agent Tshidi Bosiu Thaba" src="https://github.com/user-attachments/assets/f7ed6c20-52c0-4cd3-bbf1-84bceab4e68d" />

* **Step 126:** Assigning "View Only" role and "Support" department to Tshidi.
* <img width="1366" height="768" alt="Step 126  Giving Tshidi Bosiu Thaba View only role and adding them to the Support Department" src="https://github.com/user-attachments/assets/49f0a26f-7a33-48e6-8710-3153e17f7fc2" />

* **Step 127:** Setting appropriate access permissions for Tshidi.
* <img width="1366" height="768" alt="Step 127   Giving Tshidi Bosiu Thaba all permissions" src="https://github.com/user-attachments/assets/d2847b7c-4b83-41cf-99d1-f490fecaec44" />

* **Step 128:** Agent "Tshidi Bosiu Thaba" account successfully provisioned.
* <img width="1366" height="768" alt="Step 128  Agent Tshidi Bosiu Thaba Successfully created" src="https://github.com/user-attachments/assets/fa6298fc-992b-4d0d-9e59-6fb195e81972" />

* **Step 129:** Verifying the full list of active agents.
* <img width="1366" height="768" alt="Step 129  Viewing list of Agents" src="https://github.com/user-attachments/assets/265b811a-ed64-48aa-a3e0-28e222618317" />

* **Step 130:** Accessing the User Directory to manage end-users.
* <img width="1366" height="768" alt="Step 130  Navigated to User Directory to create users" src="https://github.com/user-attachments/assets/d8ac2348-2bb2-48fa-a68d-389e6dd799b7" />

* **Step 131:** Configuring details for user "Andile Mngxitama".
* <img width="1366" height="768" alt="Step 131  Defining details of user Andile Mngxitama" src="https://github.com/user-attachments/assets/98076f3a-78ac-4a1f-a33d-e914e3fbd7fd" />

* **Step 132:** User "Andile Mngxitama" successfully registered.
* <img width="1366" height="768" alt="Step 132  User Andile Mngxitama successfully created" src="https://github.com/user-attachments/assets/12fda3b0-4aad-4cd5-808d-e37766439fc4" />

* **Step 133:** Configuring details for user "Mubuyiseni Ndlozi".
<img width="1366" height="768" alt="Step 133  Defining details of user Mubuyiseni Ndlozi" src="https://github.com/user-attachments/assets/d89ab79d-5b66-4771-9ff3-67d5cdf907c3" />

* **Step 134:** User "Mubuyiseni Ndlozi" successfully registered.
<img width="1366" height="768" alt="Step 134  User Muyiseni Ndlozi successfully created" src="https://github.com/user-attachments/assets/2f51c01b-d556-479f-b9a7-3090c444f12d" />

* **Step 135:** Verifying the user directory list.
* <img width="1366" height="768" alt="Step 135  Viewing list of users I created" src="https://github.com/user-attachments/assets/e0740b7a-b4fc-4bae-b809-9b68941d206d" />

* **Step 136:** Accessing the Service Level Agreement (SLA) management portal.
* <img width="1366" height="768" alt="Step 136  Navigating to Service Level Agreement portal to Create SLAs" src="https://github.com/user-attachments/assets/7f4a4763-534b-4913-a6c8-a57ee0913c91" />

* **Step 137:** SLA policy created successfully.
* <img width="1366" height="768" alt="Step 137  SLA successfully created" src="https://github.com/user-attachments/assets/529cb921-9eda-45f8-97bb-bd163d48f898" />

* **Step 138:** Navigating to the Support Centre to simulate a ticket submission.
* <img width="1366" height="768" alt="Step 138  Navigating to Support Centre to lodge a ticket" src="https://github.com/user-attachments/assets/69c2bb40-e45c-4b58-88f3-e32f4baf1575" />

* **Step 139:** Submitting a support ticket as "Andile Mngxitama".
* <img width="1366" height="768" alt="Step 139  Lodging a ticket with user Andile Mngxitama" src="https://github.com/user-attachments/assets/c96f811f-8b8d-4618-88e6-41da1374281d" />

* **Step 140:** Ticket successfully submitted to the queue.
* <img width="1366" height="768" alt="Step 140  Ticket successfully lodged by user Andile Mngxitama" src="https://github.com/user-attachments/assets/dd70a5e2-2413-441e-9929-2c3d2ac58938" />

* **Step 141:** Siyolo Kamisa receiving the new ticket notification.
* <img width="1366" height="768" alt="Step 141  Siyolo Kamisa recieves notification user Andile Mngxitama has lodged a ticket" src="https://github.com/user-attachments/assets/4ead3474-ed6d-404b-b3d4-9644e4f52af2" />

* **Step 142:** Siyolo Kamisa reviewing the ticket details submitted by Andile Mngxitama.
* <img width="1366" height="768" alt="Step 142  Siyolo Kamisa opens ticket to see issue user Andile Mngxitama has" src="https://github.com/user-attachments/assets/ac843084-1a5f-4281-a935-3705ccf6a0eb" />

* **Step 143:** Siyolo Kamisa escalating/assigning the ticket to agent "Tshidi Bosiu".
* <img width="1366" height="768" alt="Step 143  Siyolo Kamisa assigns ticket to Tshidi Bosiu" src="https://github.com/user-attachments/assets/890e2b04-789a-4d9b-b5e1-9f4c10748f3a" />

* **Step 144:** Ticket assignment successfully updated.
* <img width="1366" height="768" alt="Step 144  Ticket successfully assigned to Tshidi Bosiu" src="https://github.com/user-attachments/assets/785286cf-bd22-4f8c-9a2b-36d13d23ee40" />

* **Step 145:** Tshidi Bosiu authenticating to resolve the assigned ticket.
* <img width="1366" height="768" alt="Step 145  Tshidi Bosiu logs in to resolve ticket" src="https://github.com/user-attachments/assets/22f2e9fc-3087-4b4c-ac64-110fc8d01094" />

* **Step 146:** Tshidi Bosiu documenting the ticket resolution.
"""
<img width="1366" height="768" alt="Step 146  Tshidi Bosiu notes down ticket" src="https://github.com/user-attachments/assets/cc8a44f8-45df-4df0-be80-4ac617674969" />
