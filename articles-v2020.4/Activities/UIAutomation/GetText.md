# Get Text

Get the text of the specified element. Desktop and browser are supported.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. It includes matching timeout (ms). If the time limit is exceeded and the activity has not yet been executed, an error will be thrown.

### Target

- **Control element**: Receive the variable as the target element to be got text. In terms of property, either the **control element** or the **selector** should be filled in.
- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Indicate the target area where the text is to be acquired. It can be generated automatically by clicking on the **specified element**. In terms of property, either the **control element** or the **selector** should be filled in. Only string variables and strings are supported
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Output

- **Text**: Store the text content obtained in this variable. Only string variables and strings are supported

## Operation sample

1. Drag in the **Get Text** activity and specify the element, as shown below. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/getText-1.png)

2. Open the selector window and click the "Unverified" button to check whether the specified element is recognized. Then click the "Confirm" button to close the selector window after successful recognition. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/getText-2.png)

3. Set the output text variable text: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/getText-3.png)

4. Drag in the **Confirm Message Box** activity and use the variable text as the content of the confirmation box. Click Run Flow to view the data obtained: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/getText-4.png)