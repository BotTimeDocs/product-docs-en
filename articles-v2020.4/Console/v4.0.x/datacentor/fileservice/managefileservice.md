# Manage File Service

## Folder Management

Folder Management is mainly used to create or delete various folders and subfolders. The files in File Service must be stored within a folder/subfolder.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileervice1.png)

### New Directory

Click the "New" button on the left side of the list to create a new folder, the "Name Box" of the new folder is automatically editable, enter the name and press Enter to save.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileservice2.png)

### New Subfolder

Select a folder and click the corresponding "New Subfolder" button to add a new "Subfolder" under its structure.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileservice3.png)

### Delete Folder \& Subfolder

Select a folder and click the corresponding "Delete" button to delete the folder.

## File Management

### Upload File

After selecting a folder, click the corresponding "Upload" button, select the files to be uploaded in the dialog box.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/uploadfile.png)

### File Uploading Process Management

Display the uploading process of all files, mainly including three states: uploading fully successful, uploading partially successful and uploading fully failed.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/uploadstatus.png)

### Download File

Select a folder and click the corresponding "Delete" button to delete the folder after confirming again through the dialog box.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/downloadfile.png)

### Delete File

Select a folder and click the corresponding "Delete" button to delete the folder after confirming again through the dialog box. ![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/deletefile.png)

## File Service Permission Management

File service permissions are configured according to level one folder. If a user has a certain type of permission for a level one folder, then will have the same permission for all folders or files under that level one folder.

### Open Permission Editing Page

Click the "Manage Permission" button in the operation options of level one folder to go to Permission Editing page. Click the "Save" button after the editing is completed.

![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileauthority1.png)

### Creator Permission

Creator is the creator of the folder, who is assigned the management permission by default.

### Specify User Permission

Specify User Permission can assign different user permissions for different users

1. Click the "Add" button, a dialog box will display a list of all users that can be added under the current tenant.

2. Check the users you want to add and click the "OK" button.
   
    ![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileauthority2.png)

3. The added user has read-only permission by default. You can modify the permission of a specific user by selecting from the dropdown list.
   
    ![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileauthority3.png)

4. Click the "Remove" button in front of the user name to remove the corresponding user from the specified user list.

### Other Users Permission

Other users refer to all other users under the current tenant except for the creator and the specified user list. They have no permissions by default, you can modify the permission by selecting from the dropdown list.
    ![fileservice](https://docimages.blob.core.chinacloudapi.cn/images/Console/Datacentor/fileauthority5.png)