# Import Namespace

Namespaces store different types of data, allowing you to define the scope of expressions, variables and arguments.

**Import** allows you to enter namespaces for the types that will be used in the expressions. Much like Import or Use Keywords in Visual Basic and C#, specifying namespaces in Import allows you to enter only the type name in the expression, rather than the fully qualified version type name. To open Import, please click "Import" in the editing area.

![Import](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/importnamespace20210429.png)

Import responds both to changes in the UI and to changes made when the flow is saved. After saving the flow, the namespace will be automatically added to Import. These stores include the following:

* Namespaces of all types used in variable and argument declaration.
* Namespaces of all types used in expression.
* Any other namespaces required for the serialization flow (e.g., the namespaces used by the custom activity placed in the flow).

When saving the flow, you may notice that some namespaces you have manually deleted may be automatically re-added to Import due to the logic described in the list above.

## Add Namespace to Namespace List

1. Open an automation project.

2. Click "Import" at bottom of the editing area. The import list will be displayed.

3. Enter a namespace and select a namespace from the drop-down box. When typing, a list of valid namespaces matching the typed characters will be displayed.
   
    ![Search Namespace](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/namespacelist20210429.png)

4. Press Enter to add the namespace to the list.

5. To delete a namespace from the list, please select the namespace, then right-click "Delete" or press the Delete key on the keyboard.
   
   > **Note:**
   > 
   > If a namespace is invalid for any reason (for example, the project no longer references the assembly containing the namespace), it can only be deleted.