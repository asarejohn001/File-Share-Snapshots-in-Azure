# Solution

These are the steps and configuration process I did to fulfill the objectives and solve the issue in the scenario.

## A. Create a Storage Account and File Share
1. Log into the Azure portal and access the Storage account service
   
2. Created a storage account
   
3. Chose instance details
   >[!NOTE]
   >Pick the redundancy that best matches your IT and security policy for data protection. [Lean more](https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy) about redundancy.
   
   ![Screenshot 2023-09-26 at 01 01 50](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/361f5661-83a3-4c1b-871b-483365f82f73)

4. Configured the data recovery
  ![Screenshot 2023-09-26 at 01 02 51](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/fd9b10e3-e975-47c9-9844-7ff2d653fcbe)

5. Clicked on the Fileshare blade to create a new file share
   ![Screenshot 2023-09-26 at 01 09 53](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/be2aa910-da0b-4607-b63c-09dc9d01b7f7)
   
6. Configured the file share to meet the company's IT policy
   ![Screenshot 2023-09-26 at 01 11 32](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/0769fe0a-9272-417f-8232-a60cd2c73fb6)

## B. Connect File Share to Windows VM
1. Connected to the VM where I will attach the file share and opened PowerShell as Admin
   >[!NOTE]
   >I connected to a Windows VM that I provisioned. I used a MacOS RDP application to connect to the VM via its public IP address and user credentials.

![Screenshot 2023-09-26 at 01 14 49](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/68899b39-ffb4-45a4-b0c3-f489d49d18fc)

2. Copied a script from the Azure portal that will help map the file share drive to the VM
   ![Screenshot 2023-09-26 at 01 14 05](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/1d21d381-c60a-4a8d-9a85-c9f89eeb7885)

3. Ran the script in PowerShell to perform the network map
   >[!NOTE]
   >You must make sure port 445 (Server Message Block (SMB) protocol over TCP/IP) is open for the script to run smoothly.

![Screenshot 2023-09-26 at 01 16 03](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/715df379-5883-4d97-8db5-308c8b06fa55)

4. Confirmed the successful message in PowerShell to make sure the script has run without any issues
   ![Screenshot 2023-09-26 at 01 16 45](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/80f13f4a-302e-477a-a1e1-bfd11bfcf971)


Take a Snapshot and Restore Data
