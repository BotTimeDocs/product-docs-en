# Flow Library

You can click instructions on the desktop to instruct the robot to execute flows, or use the console to centrally manage execution flows.

For details about centrally managing execution processes by the console, see: [How to issue a flow](../Console/v4.0.x/workflow/manageworkflow.md)

Locally executed flows source from:

1. Local flow files: flow packages exported from the studio (suffix: .dgs)
2. Console flow library: [flow packages](../Console/v4.0.x/packages/aboutPackages.md) used to obtain the resource group where the robot resides

The **console flow library** is only available for robots that are activated through the console.

A robot can execute only one flow at a time, and will proceed to the next flow only after the previous flow is executed.

### Executing Local Flows

1. Open a local flow library

2. Click Import Flow to import the project file (\*.dgs) exported from the studio to the local flow library.

3. Select the flow you want to execute. Here, you can enter a flow name and click Search to search for your desired flow.

4. Click Execute. The confirmation dialog box is displayed.
   
   ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/flowofexecution20201201.png)

- Flow: Displays the name and version number of the flow to be executed.

- Parameter: To input parameters for the current flow, click Execute. The dialog box asking you to input parameters is displayed.
  
  > **Description:**
  > 
  > If the parameter type is Encoo.DataType.FilePath or Encoo.DataType.FolderPath, select a file or folder path according to the parameter type, without the need of manual intervention.

- Options: Options are explained in the table below:
  
  | Options| Description      |
   | :---- | :---- |
  | Video recording| Selects whether to record a video of execution status during flow execution.|
  | Screenshot during Execution| Selects whether to take screenshot during flow execution. <br><font color="grey" size="3" face="楷体"> **Description:** <br>  <ul><li>Screenshots are saved in the Screenshots folder under the log directory of the current flow. </li><li>Name format: {flow name}-{screenshot time:YYYYMMDDHHMMSS}.jpg, for example, PaintingMaster-20201201164102599.jpg </li> </ul> </font>|
  |    Run as Administrator| Selects whether to run as an administrator. If it is selected, the program runs as an administrator; otherwise, the program runs as a normal user.|
  | Timeout| The flow is aborted when the set timeout expires. For example, when "Timeout 1min" is selected the flow needs to be executed within 1 minute. Otherwise, the flow will be forcibly aborted.



5. Click OK. The flow quickly gets ready and executes automatically. ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/running20201230.png)

### Executing Console Flow

1. Open Flow Library
2. Click Console Flow Library to obtain all flow packages from the flow library.
3. You can enter a flow package name to search for the flow package you want to execute.
4. Select the version you want to execute and click Execute. ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/Robot-Process-Console-0.png)

### Abort

A user can abort a running flow at any time.

1. Open the local/console flow library and locate a running flow.

2. Click **Abort** next to the button.
   
   > **Description:**
   > 
   > You can use the Shift+F5 shortcut key to abort the currently running flow.

3. After **Abort** is clicked, the robot will forcibly abort the running flow, regardless of where the flow goes. The **abort** operation cannot be canceled or deleted. Please be careful.
   
   ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/Robot-Process-Kill-0.png)

### Viewing logs (including recorded flow execution videos)

A user can view logs after the flow is executed.

1. Open the local/console flow library and locate a flow that was executed.
2. Click **Log** to open the log folder of this flow, including video files. ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/Robot-Process-Log-0.png)

### Deleting a Flow

A user can delete a flow in the local flow library. To delete a flow in the console flow library, go to the console.

1. Open the local flow library and select the flow to be deleted and its version number
2. Click **Delete**. A dialog box appears to ask you to confirm your deletion operation. Click OK. This version of the flow is deleted. ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Robot/robot-deleteflow-1.png)