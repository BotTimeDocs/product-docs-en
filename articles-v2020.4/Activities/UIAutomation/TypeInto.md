# Enter Text

It simulates the operation of input text to enter the text to a specified location. Desktop and browser are supported. Also, image recognition of specified elements on the desktop is supported, not on the browser yet

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. It includes matching timeout (ms). If the time limit is exceeded and the activity has not yet been executed, an error will be thrown.

### Target

- **Control element**: Receive the variable as the target element of input text. The **control element** and **selector** properties are mutually exclusive.
- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Used to indicate the target element of the text to be entered. It can be generated automatically by clicking on the **specified element**. Only string variables and strings are supported
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Input

- **Text**: The content entered to the element of the selector The text content is WYSIWYG and escaping is not supported. Only string variables and strings are supported

### Option

- **Input method**: Select the method to use when entering text. It includes three values, that is, default, keyboard simulation, and control setting. The default value of this property is **Default**. It is implemented to automatically apply the best input method based on the type of the element specified by the user (such as desktop or browser). When some scenarios cannot be executed successfully using the default property value, this property value can be manually modified to **Keyboard Simulation** or **Control Setting** to adapt to a few special scenarios to make it execute successfully.
- **Clear original text**: Clear the original data of the specified element before entering the text. It is effective only when the input method is control setting

## Operation sample

1. Drag in the **Enter Text** activity and specify an element: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setText.png)

2. Open the selector window and click the "Unverified" button to check whether the specified element is recognized. If the recognition is successful, click the "Confirm" button to close the window. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setTex-1.png)

3. Enter the text and click Run Flow to view the results: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setTex-2.png)