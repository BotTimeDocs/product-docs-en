# Confirm Message Box

The information that needs to be confirmed manually is presented in the form of a pop-up box, and the user's confirmation result (confirm, cancel) can be used to make subsequent judgments and control the direction of the flow.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Title**: The title of the pop-up confirm message box. Only string variables and strings are supported
- **Description**: The description information that needs to be confirmed in the pop-up confirm message box. Only string variables and strings are supported

### Output

- **Confirmed result**: Store the value of the confirmed result in this variable. It returns True if you click the "Confirm” button; it returns False if you click the “Cancel” button

## Operation sample

1. Drag a **Confirm Message Box** activity into the flow.

2. Double-click the **Confirm Message Box** activity in the margin to configure the property parameters. ![Confirm Message Box Configuration](https://docimages.blob.core.chinacloudapi.cn/images/Activities/comfirmsetting20201221.png)
   
   - Title: Enter the title of the confirm message box, such as "Confirm"
   - Description: Enter the description of the confirm message box, such as "Please confirm. Do you want a pop-up box?"

3. Save and execute the flow.

4. View the execution results, as shown in the figure below.
   
   ![View Execution Results](https://docimages.blob.core.chinacloudapi.cn/images/Activities/showresult20201221.png)
   
   > **Description:**
   > 
   > Select the content displayed in the pop-up box and click the right mouse button to copy it.