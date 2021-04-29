# Sequence

**Sequences** are the smallest type of project. They are suitable to linear processes as they enable you to go from one activity to another seamlessly, and act as a single block activity.

One of the key features of sequences is that they can be reused time and again, as a standalone automation project or as part of a flowchart.

Please note that due to the limitations of Windows Workflow Foundation, whenever you want to copy a large number of activities from one sequence to another, it is recommended to scroll down to the bottom of the editing area beforehand.

> **Note:**
> 
> Sequence do not use connecting lines.

## Example of a Sequence

Create an example sequence that asks the user for his name and age and then displays his answer to illustrate the sequence. The details are as follows:

1. Create a blank automation flow project. Click on "New Flow Project" in the "Start Page" to create a new project and enter a project name, such as "sequenceTest".
   
    ![Create Project](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/newflowproject20210429.png)

2. Drag the "Sequence" activity from the activities panel to the editing area
   
    ![Sequence](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/dragsequence20210429.png)

3. Create two string variables, such as Name and Age, so that you can store data from the user in them. Leave the Default field empty, to indicate that there is no default value.
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/createtwovariables20210429.png)

4. Drag two "Input Dialog" activities to the editing area, one under the other.
   
    ![Input Dialog](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/twoinputbox20210429.png)

5. Select the first "Input Dialog" and, in the properties panel, add a description asking for the username, and a custom title.

6. In the Input Content field, add the Name variable. This indicates that this variable is going to be updated with the value added by the user at this point.
   
    ![Input Dialog Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/inputbox120210429.png)

7. Repeat steps 5-6 for the second "Input Dialog" activity to ask for the user for his age, and store it in the Age variable.
   
    ![Input Dialog Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/inputbox220210429.png)

8. Add a "Confirm Message Box" activity under the second "Input Dialog".
   
    ![Confirm Message Box](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/confirmmessagebox20210429.png)

9. Select the "Confirm Message Box" and, in the properties panel, add the variables and a string to the "Description" field to enable you to display all information gathered from the user, such as Name+" is"+Age+"years old. “</br> (Optional) The "Title" field can be filled in with "User Information”
   
    ![Confirm Message Box Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/userinformation20210429.png)

10. The final sequence is shown below.
    
    ![Sample](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/finalsequence20210429.png)

Click "Run" in the run panel, type Tewin, 24, and the final result will be shown as Tewin is 24 years old.

![Result](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/sequenceresult20210429.png)