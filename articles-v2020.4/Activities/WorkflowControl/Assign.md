# Assign

Assign a value to a specified variable

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Variable name**: The name of the variable being assigned a value
- **Value**: Assigned content, which shall be of the same type as the name of the variable being assigned a value

## Operation sample

1. Drag in the **Do While** activity and create a variable count. The data type is set as Int32, and the default value is 1, and the loop condition count \<= 3 is added, as shown below. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/dowhile-1.png)

2. Double-click to open the activity and drag the **Assignment** activity to the Do While container. Set the count to increment, such as count = count + 1: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/dowhile-2.png)

3. Drag in the **Write to Log** activity and enter the printing content: "Loop count: “+ count.ToString(). Click Run Flow to view the output log: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/dowhile-3.png)