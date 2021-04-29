# Variables List

The Variables List can be used to create and modify variables.

![Variables List](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/variables20210429.png)

| Field| Description
|----------|----------
| Name (Required)| The name of the variable. If no name is added to the variable, one will be generated automatically.
| Variable Type (Required)| Enables you to choose the type of variable. The following options are available: </br> Boolean </br> Int32 </br> String </br> Object </br> Array of \[T] </br> System.Data.DataTable </br> BotTimeUI.Common.Control.Interface.IUiObject </br> Browse .Net Type
| Scope (Required)| The area in which a variable is available, such as a specific activity. </br> By default, they are available in the entire project.
| Default Value (Optional)| The default value of the variable.  </br> If this field is empty, the variable is initialized with the default value of its type. For example, for an Int32, the default value is 0.

> **Note:**
> 
> 1. The scope of the variable, if set to local, simply indicates that the variable exists in the current scope, but the variable name needs to remain globally unique.
> 
> 2. The system reserved words are not allowed to be used in the variable name. For example, add, delete, etc.

## Variable Context Menu

![Menu](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/variablemenu20210429.png)

| Field| Description
|----------|----------
| Delete| The variable shall be removed from the list but not from the flow.
| Add Comment| Open the "Add Comment" window to add comments to the variable.
| Edit Comment| Open the "Add Comment" window and make changes to existing comments.
| Delete Comment| Delete the comments added for the variable.

