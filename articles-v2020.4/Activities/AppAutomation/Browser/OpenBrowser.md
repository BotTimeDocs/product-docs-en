# Open Browser

Use this activity to open the specified URL with a browser.

This activity is also often used as a container. Some other web action activities are often placed in this activity to complete.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When Yes is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when No is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported.

### Target

- **Browser type**: The type of the opened target browser, such as Chrome, IE.
- **URL**: This URL will be opened, and only string variables and strings are supported.

### Output

- **Browser**: Store the opened browser type object to this variable. It can be used as input for the next browser activity.

### Option

- **Open method**: When the browser type is Chrome, Firefox, and Edge, the available open methods are Native and Selenium (WEB automation tool).

- **Wait for loading to complete**: When it is selected, wait for the target user interface element to complete loading before executing the next activity operation.

- **Close when completed**: When it is selected, the browser will be closed automatically when this activity is completed.
  
  > **Note:**
  > 
  > If the silent running method is used, please determine whether to select this option according to the situation, otherwise, you cannot bind the browser.

- **Silent run**: When "Selenium" is selected as the open method and the "Silent Run" option is selected, the flow can be run with a separate browser open and unseen, so that the user can operate the browser manually and independently. \-->

- **Maximization**: When it is selected, the browser specified by you can be automatically maximized for subsequent operations.

## Operation sample

1. Drag the **Open Browser** activity into the project flow: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenBrowser20201221-01.png)

2. Select the browser type and enter the URL: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenBrowser20201221-02.png)

3. Click Run to view the results: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenBrowser20201221-03.png)