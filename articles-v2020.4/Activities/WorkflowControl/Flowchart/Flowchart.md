# Flowchart

Flowcharts can contain various activities and the activities can be connected by connecting lines. The flowcharts have a wide range of applications and are reusable.

Unlike sequences, the flowcharts present multiple branching logical operators, that enable you to create complex business flows.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Option

- **Validate unconnected activities**: Whether to validate activities that are not connected in the flow

## Operation sample

1. Drag the **Flowchart** activity into the project flow: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/flowchart-1.png)

2. Double-click to open it, and drag in other activities to the **Flowchart** activity. For example, drag in the **Confirm Message Box** activity, as shown in the following figure. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/flowchart-2.png)