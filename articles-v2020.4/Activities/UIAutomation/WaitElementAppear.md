# Wait for element to appear

Wait for the specified UI element to appear from the screen. Desktop and browser are supported. Also, image recognition of specified elements on the desktop is supported, not on the browser yet

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. It includes matching timeout (ms). If the time limit is exceeded and the activity has not yet been executed, an error will be thrown.

> **Note:**
> 
> The **"Timeout"** property setting needs to be set as needed, otherwise, the default is the project's timeout (30 seconds). For example, if we set the matching timeout to 5000 (milliseconds) and the timeout to 20000 (milliseconds), when executing, we will wait for the target element in a loop every 5000 (milliseconds) until we reach the "timeout" time (20000 milliseconds) before continuing to execute

### Target

- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Used to indicate a specific UI element. The activity will wait for the element specified by this selector to appear. It can be generated automatically by clicking on the **specified element**. Only string variables and strings are supported
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Output

- **Result**: The result (success/failure) of the execution of this activity is stored in this variable. When the specified target appears, the stored value is True. Only Boolean variables and Booleans are supported
- **Control element**: The element to appear is stored in this variable. An activity such as **Wait for Element to Disappear** can be used as the input value. When the element is specified using image recognition, an anchor element instead of an image element is returned

## Operation sample

1. Drag in the **Wait for Element to Appear** activity and set the corresponding property value: ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/WaitElementAppear/Appear1.png)

2. Specify an element and validate the existence of the element: ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/WaitElementAppear/Appear2.png)

3. Run the flow and view the results: ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/WaitElementAppear/Appear3.png)
