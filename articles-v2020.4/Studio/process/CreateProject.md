# Create Flow Project

## Flow Project

A **flow project** is a collection of all flow files related to a single automation job. For example, if you need to create an automation flow that handles customer orders on a regular basis, you can create a flow project in which all subflow files, dependencies, and other information related to this job will appear. Flow project is the basic unit that you develop, publish, and deploy to robots for running. Typically, a new flow project shall be created for each separate job.

After you enable the studio and create a new project, the project will be stored under the default path `-%USERPROFILE%\Documents\Encoo`.

The project includes the following two parts.

- Main.xaml flow file created automatically. This file serves as the start file when the flow is executed and contains the main flow of the studio.
- Other .xaml flow files. These files need to be linked to the Main.xaml file by the [Call Flow](../../Activities/WorkflowControl/InvokeWorkflow.md) activity, because when the automation flow is run or debugged, it will start from the Main.xaml file.

## Create Flow

This example will teach you how to create and run a basic flow project. We will open the browser, search the weather forecast for tomorrow's weather information, and make an alert about whether it's going to rain tomorrow.

1. Open ENCOO RPA Studio
2. Create a new project and enter the project name (take MyFirstProject as an example) </br>. 
   UIA3 is recommended for the **Desktop Recording Technology** selection under Advanced Settings.
   
    The difference between UIA3 and UIA lies in the different levels of support for different technologies. </br>
   
   - For WPF and Windows Store Apps, UIA 3 has a higher support level.
   
   - For C# and WinForms, UIA has a higher support level.
     
     > **Note:**
     > 
     > UIA3 and UIA cannot be used in the same project at the same time.
   
    ![Create Project](https://docimages.blob.core.chinacloudapi.cn/images/Studio/typeOfWorkflow/myfirstproject20201019.png)

3. Search for the "Open Browser" activity in the activities panel and drag it into the editing area to connect to the Start node

4. In the properties panel of the activity, enter the following content.
   
   - Browser type: IE
   - URL: "https://www.baidu.com"
   
    ![Open Browser](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/intoOpenBrowser.PNG)

5. Double-click the "Open Browser" activity and click "Smart Recording" under the Menu Bar - Tools to open the recorder

6. Open the home page of the Baidu website in IE browser, and then click "Smart Recording" in the recorder to record the website operations
   
    ![Record](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/baidu.PNG)

7. Click on the search text box on the home page of Baidu and enter the words you want to search in the pop-up box that appears (take weather as an example)
   
    ![Enter Text](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/inputTianqi.PNG)

8. Click on Baidu Searches, or press Enter
   
    ![Baidu Searches](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/clickBaidu.png)

9. Open the recorder interface and select "Text" -> "Get Text". When a yellow rectangle box appears, click on tomorrow's weather information to get the weather text
   
    ![Get Text](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/getText.png)

10. Press the shortcut key "Esc" on the keyboard to end the recording of website operations

11. Click "Save \& Exit" in the recorder to save the recorded automation flow to the studio
    
    ![Save Flow](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/saveExit.PNG)

12. Open the variable list and create a String variable-weather to store the obtained weather text
    
    ![Create Variable](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/createVariable.PNG)

13. Select the "Get Text" activity, and in the properties panel, enter the following content:
    
    - Text: weather
    
    ![Input Variables](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/inputWeather.PNG)

14. Drag a "Conditional (If)" activity from the activities panel to connect to the "Get Text" activity, and in the properties panel of the activity, enter the following content:
    
    - Judgment condition: weather.Contains("rain")
    
    ![Drag in Conditional Activity](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/intoIf.PNG)

15. Drag a confirm message box activity into the Then section of the condition, and in the properties panel of this activity, enter the following content:
    
    - Title: "Tomorrow's Weather Alert"
    - Description: "It's going to rain tomorrow, so don't forget to bring your umbrella."
    
    ![Drag in Confirm Message Box](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/intoInput.PNG)

16. Drag another confirm message box into the Else section of the condition, and in the properties panel of this activity, enter the following content:
    
    - Title: "Tomorrow's Weather Alert"
    - Description: "No rain tomorrow. You can go out for a walk"

## Run Flow

1. Click "Run" to try to run the automation flow
   
    ![Run Project](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/runflow20201019.png)

2. During the runtime, the studio will automatically replay the recording process and alerts you whether it's going to rain tomorrow
   
    <!-- ![运行结果](https://docimages.blob.core.chinacloudapi.cn/images/Studio/automationProject/createProject/result.png) -->
