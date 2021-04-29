# Reference Project

**Reference Project** is used to reference an external project to the current project as a dependency of the current project, and the dependency is called in the current project through the **Call Flow (Reference Project)** activity.

## Operation example

1. In the editing page of Studio, right click the project name and select **Reference Project > Select File** in the pop-up menu. 

![image-20201207160513550](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/referenceproject20210428.png)

2. In the Open File dialog, select the project file in dgs format that needs to be referenced.
   
   > **Description:**
   > 
   > - The dgs format file is the project file that is generated when the project is exported.
   > - When the project file is selected, it is in the **Dependencies** under the current project.
   
   ![image-20201207161108502](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/referencedependency20210428.png)

3. In the newly created flow where you need to reference a flow, drag in the **Call Flow (Reference Project)** activity.
   
   ![image-20201207161253694](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/invokeworkflowview20210428.png)

4. Double click the **Call Flow (Reference Project)** activity to configure it: Select the flow to be called and the flow master file, as shown below.
   
   > **Description:**
   > 
   > (Optional) Click the "Set Arguments" button to set arguments for the currently called flow.
   
   ![image-20201207161408189](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/invokeworkflow20210428.jpg)

5. Save the flow (Ctrl + S) and run it (Ctrl + F5).