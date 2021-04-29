# Variable

In ENCOO RPA Studio, **variables** are used throughout the automation flow to store multiple types of data. Another key aspect of variables is that their value can change so that you can control how many times the body of a loop is executed.

> **Note:**
> 
> Variables need to be created with different names, even if used in different Scopes.

The data stored within a variable is called a value, and it can be of multiple types. In ENCOO RPA Studio, we support a large amount of types, ranging from text, number, time and date, to any variable type.

## Create Variable

![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/variables20210429.png)

> **Note:**
> 
> Variables cannot be created if the editing area does not contain at least one activity.

### Create variables with Ctrl+B shortcut key

- **From Activities**

1. From the Activities panel, drag an activity to the editing area. Fill in the variable name in the input box of the activity.

2. Select and right click the name, select "Create Variable" from the context menu, or press **Ctrl+B** shortcut key, the variable is created. Check its type and scope in the Variables list.
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/fromactivitycreate20210429.png)

- **From the Properties Panel**

1. In the Properties panel of any activity, select a property, and fill in the variable name in the input box.

2. Select and right click the name, select "Create Variable" from the context menu, or press **Ctrl+B** shortcut key, the variable is created. Check its type and scope in the Variables list.
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/frompropertiescreate20210429.png)

- **From Expression Editor**

1. Select any activity, open the expression editor of any property of the activity, and fill in an expression.

2. Select and right click a part of the expression, select "Create Variable" from the context menu, or press **Ctrl+B** shortcut key, the variable is created. Check its type and scope in the Variables list.
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/fromexpressioneditor20210429.png)

> **Note:**
> 
> For the variable created with shortcut key, the type is automatically generated depending on the selected property.

### Create Variable from Context Menu

1. Right click the current activity to bring up the context menu and click "Create Variable".
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/menu-createVariable.png)

2. Fill in the name and press Enter. You can view and edit it in the Variables list. The scope of such variables is the smallest container it is part of.

> **Note:**
> 
> The default type of variables created from the context menu is String.

### Create Variable from Variables List

1. In the editing area, click "Variables". The "Variables" list is displayed.
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/variablePanel-createVariable.png)

2. Click "Create Variable", a new variable with default field value is displayed.

> **Note:**
> 
> The default type of all new variables created from "Variables List" is String.

## Delete Variable

1. In the Variables List, select and right click a variable. Click "Delete" in the context menu.
   
    ![Delete Variable](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/deleteVariable.png)

2. In the Variables List, select a variable and press Delete.

> **Note:**
> 
> To undo this operation, press Ctrl + Z.

## Search Variable

When variables are used in multiple places in multiple flow files and you need to find and locate them, you can search them from the Quick Search box in the menu bar or from the **View > Search** menu.

![Search and Locate Variable](https://docimages.blob.core.chinacloudapi.cn/images/Studio/searchvariables20210323.png)

Enter the variable to be searched in the search box to find and locate the specified variable in all flow files.

> **Description:**
> 
> In the upper right corner of the search results, select corresponding option from the drop-down list to search in "All Files" and "Current File".

![Search Results](https://docimages.blob.core.chinacloudapi.cn/images/Studio/searchvariablesresult20210323.png)

## Browse .Net Variable Type

To search for types of variables that are not displayed by default in the "Variable Type" list, do the following:

1. In the Variables list, from the "Variable Type" drop-down list, select "Browser Type". The "Browse and Select a .Net Type" window is displayed.
   
    ![Browser Type](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/viewTypeOfVariable.png)

2. In the "Type Name" field, type a keyword for the variable you are looking for, such as table.
   
    ![Enter Variable Type](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/inputTable.png)

3. Select table type and click "OK". The variable type is displayed in the "Variable Type" drop-down list.
   
    ![Select Type](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Variable/confirmTable.png)

> **Note:**
> 
> After first using a variable type from the "Browse and Select a .Net Type" window, it is displayed in the "Variable Type" drop-down list, in the Variables list.