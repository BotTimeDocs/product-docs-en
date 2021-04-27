# Flow Decision

An activity which executes one of two branches, depending on whether a specified condition is met. This activity can only be used in a Flowchart and is equivalent to the “Condition” activity.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Decision condition**: Boolean expressions

### Miscellaneous

- **False label**: The decision is False, and you can customize the decision name
- **True label**: The decision is True, and you can customize the decision name

## Operation sample

1. Drag in the **Wait for Element to Appear** activity, specify the element, and add the output variable isTrue. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/decision-1.png)

2. Drag in the **Flow Decision** activity and use the output variable isTrue from the previous step as the input condition. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/decision-3.png)

3. Drag in two **Write to Log** activities, attach them to the True and False ends of the decision activity respectively, and add a prompt as to whether the element appears. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/decision-2.png)

4. The web page for the element specified in step 1 remains open. Run the flow and view the prompt in the output window. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/decision-4.png)