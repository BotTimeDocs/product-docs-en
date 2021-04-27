# If

It determines the next step of execution depending on whether the specified condition is met

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Judgment condition**: Boolean expressions

## Operation sample

1. Drag in the **Get Structured Data** activity, specify the table element on the web (for example, [a stock website](http://stockpage.10jqka.com.cn/1A0001/#refCountId=stockpage_5c3e9aef_93)), and set the output variable. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/if-1.png)

2. Drag in the \*\*if\*\* activity and set the judgment condition dt.Rows.Count == 10 (to check if the data table has 10 rows of data). ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/if-2.png)

3. Double-click on the **if** activity, drag in two **Write to Log** activities to the if container, and write them into different log texts according to the True/False judgment conditions, respectively. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/if-3.png)

4. Click Run Flow and view the run results. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/if-4.png)