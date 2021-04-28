# Parameter List

The parameter list can be used to create and modify parameters.

![Parameter](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/createparameter20210428.png)

| Field| Description
|----------|----------
| Name (Required)| The name of the parameter. If no name is added to the parameter, one will be generated automatically.
| Direction (Required)| Select a direction for the parameter. The available options are as follows: </br> Input - This parameter can be used only for the given project; </br> Output - This parameter can be used to pass data outside the given project; </br> Input/Output - These parameters can be used both inside and outside the given project; </br> Property - This parameter is not being used currently.
| Parameter Type (Required)| Select the type of value you want the parameter to store. The available options are as follows: </br> - Boolean: Boolean </br> - Int32: 32-bit integer </br> - String: string type </br> - Object: object </br> - Array of \[T]: array </br> - System.Data.DataTable: an in-memory data table </br> - BotTimeUI.Common.Control.Interface.IUiObject </br> - Encoo.DataType.FilePath: open the file </br> - Encoo.DataType.FolderPath: open the directory </br> browser .Net type </br> If .Net type is selected from the "Browse and Select .Net Type" window, it will be added to the "Parameter Type" drop-down box.
| Default Value (Optional)| The default value of the parameter. If this field is empty, the parameter has no default value.

> **Note:**
> 
> The system reserved words are not allowed to be used in the parameter name. For example, add, delete, etc.

## Parameter Context Menu

![Menu](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/argument20210428.png)

| Field| Description
|----------|----------
| Delete| The parameter shall be removed from the list but not from the flow.
| Add Comment| Open the "Add Comment" window to add comments to the parameter.
| Edit Comment| Open the "Add Comment" window and make changes to existing comments.
| Delete Comment| Delete the comments added for the parameter.

