# Flowchart

The **flowchart** can be used in a variety of situations. It can be used repeatedly in projects from large to small.

Unlike sequences, the most important aspect of the flowchart is its applicability to more complex business logic. You can use several different logical operators to integrate automation projects in a more diverse, quick, and easy way.

## Flowchart Example

Create an example of determining user login to illustrate the flowchart. The details are as follows:

1. Create a blank automation flow project. Click on "New Flow Project" in the Start Page to create a new project and enter a project name, such as "flowTest".
   
    ![Create Project](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/createflowchart20210429.png)

2. Click "Variables" in the editing area to bring up the list of variables, and click "Create Variable" to create two string variables (name, password).
   
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/createnamepasswordvariables20210429.png)

3. Add the "Flowchart" to the editing area and connect it to the "Start" node. In the properties panel of the activity, enter the following content:
   
   * Display name: "User Login"
   
    ![Flowchart](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/displayname20210429.png)

4. Double-click to open the flowchart, add the "Input Dialog" to the flowchart, and connect it to the "Start" node.
   
    ![Input Dialog](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/inputdialog20210429.png)

5. In the properties panel of "Input Dialog", enter the following content:
   
   * Input content: name
   * Title: "Username"
   * Description: "Please enter your username"
   * Display name: Enter your username
   
    ![Input Dialog Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/property20210429.png)

6. Add the "Flow Decision" to the editing area and connect it to the "Input Dialog". This activity can be used to determine whether the username entered by the user is correct.
   
    ![Flow Decision](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/flowdecision20210429.png)

7. In the properties panel of "Flow Decision", enter the following content:
   
   * Judgment condition: name == "". This field is used to determine if the username is empty
   * Display name: Determine if the username is empty. This field can be changed to any other content you want
   
    ![Flow Decision Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/flowdecisionproperty20210429.png)

8. Add an "Input Dialog" and connect it to the False branch of the flow decision. The True branch of the flow decision is connected to the previous "Input Dialog" and is used to re-enter the username.
   
    ![Input Dialog](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/decision20210429.png)

9. In the properties panel of "Input Dialog", enter the following content:
   
   * Inputted content: password
   * Title: "Password"
   * Description: "Please enter your password"
   * Display name: Enter your password
   
    ![Input Dialog Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/inputpassword20210429.png)

10. Add a "Flow Decision" and connect it to the "Input Dialog". This activity can be used to determine whether the password entered by the user is correct.
    
    ![Flow Decision](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/decision220210429.png)

11. In the properties panel of "Flow Decision", enter the following content:
    
    * Judgement condition: password == "". This field is used to determine if the password is empty
    * Display name: Determine if the password is empty. This field can be changed to any other content you need.
    
    ![Flow Decision Properties](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/decision2property20210429.png)

12. Add a "Confirm Message Box" and connect it to the False branch of the flow decision. The True branch of the flow decision is connected to the previous "Input Dialog" and is used to re-enter the password.
    
    ![Confirm Message Box](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/con20210429.png)

13. In the properties panel of "Confirm Message Box", enter the following content:
    
    * Title: "User Login"
    * Description: name+"Login Successful"

14. The final flowchart is shown below.
    
    ![Sample](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/UserLogin20210429.jpg)

Click "Run" in the run panel, enter your username and password, and Tewin Login Successful will be shown in the final result.

![Result](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/userloginresult20210429.png)