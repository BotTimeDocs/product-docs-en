# Execute C# Code

It provides a C# code editor and supports writing C# class, function, and other basic codes. The variables defined in the editor can be directly used, without the need for parameter passing between the editor and C# code editor.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

## Operation sample

1. Drag the **Execute C# Code** activity into the flow.

2. Double-click on the activity's blank space to bring up the file path that has been populated by default and the Edit Code button.
   
    ![CSharpUI](https://docimages.blob.core.chinacloudapi.cn/images/Activities/CSharp20201211.png)
   
   - File path: Click the "..." button, select the path to the C# file and open it, such as Dworkspace\\Encoo\\activityflow\\code\\CSharp\\executeCSharpcode.cs
   
   - Edit Code: Click the "Edit Code" button and enter the C# code snippet to be executed in the C# code editor as shown in the following figure.
     
       > **Description:**
       > 
       > Variable references are supported here, and variables `m` and `n` of type String are defined in the editor beforehand.
     
       ![Execute C# Code Snippet](https://docimages.blob.core.chinacloudapi.cn/images/Activities/executecsharpcode20210303.png)

3. Save and execute the flow.

4. View the run results in the output window.
   
   ![Operation Result](https://docimages.blob.core.chinacloudapi.cn/images/Activities/executecsharpresult20210303.png)