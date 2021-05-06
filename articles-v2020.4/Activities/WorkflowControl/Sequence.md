# Sequence

It enables you to create linear flows comprised of many activities, which are executed in sequential order. It can either serve as a stand-alone automation project or can be included as part of a flowchart, to help you group specific activities.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

## Operation sample

1. Drag the **Sequence** activity into the project flow:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/sequence20210506.png)

2. Double-click to open the activity and drag any other activities into the sequence container as shown below:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/doubleclicksequence20210506.png)