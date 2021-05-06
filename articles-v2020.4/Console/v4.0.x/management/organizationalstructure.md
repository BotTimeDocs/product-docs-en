# Organizational Structure Management

Organizational Structure Management is mainly used to manage the departments and users in the company, which can also simultaneously control various permissions of the related departments, users, and robots.

Here, creating a department and configuring the department information is taken as an example. The steps are as follows:

## Prerequisites

A **system administrator** has created a company (that is, tenant) in the management backend of the console.

## Creating Department

Create a department for the created company.

1. In **Global Management > Organizational Structure Management** of the ENCOO RPA console, click "+" to create a department.
   
    ![Creating Department](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user1.png)

2. Click the "OK" button to confirm the creation of a department or sub-department.

## Invite User

Invite users for the created department.

1. In "User Management" tab, click "**+Invite User**" to add user information for the selected department.
   
   ![Add User](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user2.png)

2. (Optional) Click the "**Add and Continue Adding**" button to save the added user and continue adding a new user.

3. Click the "**Save**" button. You can view information about added users on the user information list page.
   
   ![User Information List](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user4.png)

4. (Optional) To view, change, or delete an added user, click the corresponding option in the "Action" bar.
   
   ![Available Actions for Added Users](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user5.png)
   
   - **View**: View information about added users and edit the relevant information of "User Name" and "Remarks".
   
   - **Change Department**: Move the added users to another department in the organization structure.
   
   - **Change Role**: Change roles for added users. For details about roles, see the table below.
     
     | Role| Menu Permissions| Function Permissions
     |----------|----------|----------
     | Enterprise Administrator| Organizational Structure Management| Has add, modify and delete permissions under this menu
     | \-| Organizational Structure Management > User Management| Has add, modify and delete permissions under this menu
     | \-| Audit Log| Has add, modify and delete permissions under this menu
     | \-| License| Has add, modify and delete permissions under this menu
     | \-| Open menu in the "Function Configuration" corresponding to the department| Has add, modify and delete permissions under this menu
     | Organizational Structure Administrator| Organizational Structure Management| Has add, modify and delete permissions under this menu
     | \-| Open menu in the "Function Configuration" corresponding to the department| Has add, modify and delete permissions under this menu
     | Audit Log Administrator| Audit Log| Has add, modify and delete permissions under this menu
     | \-| Open menu in the "Function Configuration" corresponding to the department| Has add, modify and delete permissions under this menu
     | Common User| Open menu in the "Function Configuration" corresponding to the department| Has add, modify and delete permissions under this menu

   
   - **Delete**: Deletes the added users in this tenant.

## Configuring Department Data Permissions

The "**Data Permission Config**” tab is mainly used for configuring the data permission for the selected departments. The system will, by default, inherit the data permission of the superior department for the created departments.

1. To configure department data permissions, click the "Edit" button in the upper right corner of the page.
   
   ![Configuring Department Data Permissions](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user6.png)
   
   - **Department Configuration Information**
     - Owner: By default, it is the creator of the current department and can be changed.
     - Department: The organizational relationship of the current department.
     - Manager: The owner of the superior department will automatically become the manager of the current department. It is mainly divided into enterprise managers or organizational structure managers.
   - **Data Permission Mode**:
     - Whether to inherit superior permission: If you choose "Inherit Superior Permission", the system will calculate the final permission according to the custom permission and the inherited superior permission.
     - User Permission: Configures user access to resources in the department.

     ![Menu Function Permissions](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user10.png)
       
     - Robot Permission: Configures user access to the specified robot in the department.
     - API Key access: Configures API KEY access to resources to control access to URLs that use the API KEY.

2. Click the "Save" button to save the configured department data permissions.

## Configuring Menu Function Permissions

Enables the specified menu function permissions for the selected department.

1. To configure department menu function permissions, click the "Edit" button in the upper right corner of the page.
   
    ![Menu Function Permissions](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4user13.png)

2. Click the "Save" button to save the configured department menu function permissions.

## Follow-up Actions

- **View organization structure**: On the "Organizational Structure Management" page, you can view the current organization structure list of the current company.
- **Modify department information**: On the "Department Information Config" page, click the "Edit" button to modify the current department information.
- **Delete department information**: On the "Organizational Structure Management" page, select and click the "Delete" option next to the department, and delete the current department.
- **Create sub-department**: On the "Organizational Structure Management" page, select and click the "Create Sub-department" next to the department to create a sub-department for the current tenant or department.