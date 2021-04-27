# Application Management

Go to **Application Management** and you can see all the published applications under the current department. You can switch **Department** to see the applications under different departments.

## View Application

The application list will list all published applications and their current states.

- **Enabled**: It means that the current application has been published, and the users under the department can view and run the application by visiting **Application Center > My Applications**.
- **Disabled**: It means that the current application has been unpublished, and it is not visible to users.

The enabled application will be marked with its currently enabled version number. You can click the application name to view the application details.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/manageapps.png)

## View Application Details

Click the application name to open the application details.

In the Application Details, you can view the current and historical versions of the application. The currently enabled version will show the **Current** marker at the version number. You can also try the current version of the application on the details page.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/appsdetail.png)

Click **View More Versions** to view other versions of the application. The current preview version is marked with an arrow. You can switch to the current preview version by clicking the version number.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/appsdetail2.png)

If you want to switch the currently enabled version of the application, you can switch to the details of the version you want to enable through **View More Versions**, and click **Switch to Current Version** in the details to switch the enabled version of the application to the currently selected version.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/appsdetail3.png)

> **Description:**
> 
> The disabled application does not have a currently enabled version because it has not been published.

## Enable Application

For the **Disabled** application, you can enable the application through the Enable button in the list or the Details. By default, when the application is enabled in the list, the latest version of the application is enabled.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/activeapps1.png)

When the application is enabled in the Details, the currently selected version in the Details is enabled by default.

## Disable Application

For the **Enabled** application, you can disable the application through the Disable button in the list or the Details.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/inactiveapps1.png)

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/inactiveapps2.png)

## Delete Application

You can delete a single version or the entire application.

When you delete the entire application, all versions of the application will be deleted and the original development package of the application will be deleted as well.

### Delete Application

Go to Application Management page, find the application you want to delete, click Delete, and delete it after confirming again.

![package](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/deleteApps.png)

### Delete Application Version

Go to the Application Management page and find the application where the version you want to delete is located. Click it in the Application Details to view the version. Locate the version you want to delete, and click Delete to delete it.

![package](https://docimages.blob.core.chinacloudapi.cn/images/Kris/AppsV2/deleteApps1.png)

It is necessary to meet the following conditions for deleting versions:

- The version is not at the Current state.