# Preview Data Table

Preview the specified input data table, that is, present the data content of the data table in the form of an interface at runtime

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Data table**: The data in this data table will be presented in the form of an interface

## Operation sample

1. Drag the **Build Data Table** activity into the project flow: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/BulidDataTable20201224.png)

2. Double-click to open the Build Data Table builder and edit the column information and row values. Create a variable of the DataTable type to store the output data table, such as table, as shown below. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/BulidDataTable2020122402.png)

3. Drag in the **Preview Data Table** activity and fill in the data table variable table already built above. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/BulidDataTable2020122403.png)

4. Click Run and view the results. Check if the previewed data table is consistent with the data table built. ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/BulidDataTable2020122404.png)