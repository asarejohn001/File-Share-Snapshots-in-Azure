# Solution

These are the steps and configuration process to fullfill the objecives and solve the issue in the scenario.

## A. Create a Storage Account and File Share
1. Log into the Azure portal and access the Storage account service
2. Create a storage account
3. Chose your instance details
   ![Screenshot 2023-09-26 at 01 01 50](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/361f5661-83a3-4c1b-871b-483365f82f73)
   >[!NOTE]
   >Pick the redundancy that best match your IT and securit policy for data protection. [Lean more](https://learn.microsoft.com/en-us/azure/storage/common/storage-redundancy) about redundancy.
4. Configure the data recovery
  ![Screenshot 2023-09-26 at 01 02 51](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/fd9b10e3-e975-47c9-9844-7ff2d653fcbe)
5. Click on the Fileshare blade to create a new fileshare
   ![Screenshot 2023-09-26 at 01 09 53](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/be2aa910-da0b-4607-b63c-09dc9d01b7f7)
6. Configure the file share to meet your company's IT policy
   ![Screenshot 2023-09-26 at 01 11 32](https://github.com/asarejohn001/File-Share-Snapshots-in-Azure/assets/137245223/0769fe0a-9272-417f-8232-a60cd2c73fb6)



 
## B. Connect File Share to Windows VM
1. Connect to the VM where you will attac
Take a Snapshot and Restore Data
