# Step-by-Step Debugging

## Debug Single File

When an automation project is complex and each debugging or running is time and labor intensive, you can use **Debug/Run File** to split a large project and debug or run it separately. In this way, the correctness of the project can be judged more quickly and the project can be verified more quickly.

You can use the right-click menu in the project panel or the shortcut (F6/Ctrl+F6) to debug or run the file. ![Entry for Step-by-step Debugging](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/partialdebug20210222.png)

When the currently selected flow file contains arguments, click "Debug/Run File", a dialog box will appear to set the flow arguments, you can choose to set different argument values for verification, or use the default values for verification.

![Open File/Folder](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/openfile&folder20201214.png)

> **Note:**
> 
> - The Set Flow Arguments window only supports to change the values of In arguments.
> - When the argument type is `Encoo.DataType.FilePath` or `Encoo.DataType.FolderPath`, you can click the icon as shown above to open and enter the path to the file or folder.

## Debug Single Activity

During the implementation of automation projects, it is often encountered that an activity has been located to have an error exception, but cannot be more accurately located to a specific step of the activity error, you can select the activity in the flow, and select "Activity Debugging" in the right-click menu to debug the selected single activity.

> **Description:**
> 
> When using the "Activity Debugging" function in the context menu, setting the values of variables or arguments is supported.

![Entry for Debugging Single Activity](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/debugactivity20210317.png)

When the currently selected activity contains variables or arguments, a pop-up box will display the variables and arguments of the activity's scope. (Optional) After setting the variables or arguments in the pop-up box, click the "OK" button to start debugging the activity.

![Setting Box for Debugging Single Activity](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/debugactivityarguments20210317.png)

## Start Debugging from Selected Activity

In Studio, if there are multiple activities in the flow and you need to specify an activity to start debugging from, you can select the activity you need to start debugging from in the editing area and select the **Debug from This Activity** option in the right-click shortcut menu, which will start debugging the flow from the selected activity.

> **Description:**
> 
> When using the "Debug from This Activity" function in the context menu, setting the values of variables or arguments is supported.

![Debug from Selected Activity](https://docimages.blob.core.chinacloudapi.cn/images/Studio/debugformactivity20210323.png)