# Send Shortcut

It simulates the behavior of a human pressing a shortcut key at the keyboard and is mainly used to send keyboard shortcuts to a specified UI element. It also enables you to send shortcut keys without specifying an element (For example, both selector and control element properties are empty). Desktop and browser are supported. Also, image recognition of specified elements on the desktop is supported, not on the browser yet

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. It includes matching timeout (ms). If the time limit is exceeded and the activity has not yet been executed, an error will be thrown.

### Option

- **Pre-send action**: the action before sending the shortcut. Both click and set focus actions are supported.

### Target

- **Control element**: Receive the variable as the target element to receive the shortcut. The **control element** and **selector** properties are mutually exclusive and can both be empty
- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Used to indicate the target position to receive the shortcut. It can be generated automatically by clicking on the **specified element**. The **control element** and **selector** properties are mutually exclusive and can both be empty. Only string variables and strings are supported.
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Auxiliary Key

- **Alt**: When this box is checked, it simulates clicking this key
- **Ctrl**: When this box is checked, it simulates clicking this key
- **Shift**: When this box is checked, it simulates clicking this key
- **Win**: When this box is checked, it simulates clicking this key

### Input

- **Key-value**: It simulates clicking this key. Multiple key-values are supported. For example, if "A, Z" needs to be pressed at the same time, fill in "AZ"

## Operation sample

1. Drag in the **Set Clipboard Text** activity and set the input text. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/sendHotkey-1.png)

2. Drag in the **Send Shortcut** activity, specify the element, and set the key-value CTRL+V. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/sendHotkey-2.png)

3. Click Run Flow and view the flow run results. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/sendHotkey-3.png)
   
   > **Description:**
   > 
   > This flow can be used in many scenarios to replace the "Enter Text" activity, and it runs efficiently and is less prone to errors in entering text.