# Project Settings

**Project Settings** is used to set the property values related to the running and debugging of activities of a category and apply them to all activities of that category in the project.

## Set Activity Properties

How to set the properties of activities of a category?

You can right click the Project folder in the Project panel, open the menu, then click "Project Settings", to open the "Project Settings" window.

![Project Settings Window](https://docimages.blob.core.chinacloudapi.cn/images/Studio/typeOfWorkflow/itemsettings20201019.png)

**Project Settings** window displays the categories in which the activity properties can be set at the left side. For example, the activity property values set for automation will be applied to all activities related to automation.

**Project Settings** window displays the specific properties of corresponding category at the right side. Once corresponding property value is set, the set value will be used for running or debugging the relevant activities in the project.

**Restore Default Value** enables you to restore the property values set for the current category to their default values with one click.

In the project, if a property value is set in the **Properties Panel**, the value set in the Properties Panel will overwrite the value set in **Project Settings**, and the value set in the Properties Panel will be used for running or debugging the project.

For example, set the **Browser Type** property of **Open Browser**: </br> In Project Settings, set the property value of **Browser Type** to Chrome; in Properties Panel, set the property value to FireFox, when the project is executed, a URL will be opened with Firefox.

![Set Activity Properties](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/projectSettings/settingValue.png)

> **Note:**
> 
> The property values set in Project Settings are not updated in the Properties panel.
> 
> If the .settings folder is renamed or deleted, it will be automatically created by default when running or debugging the project.