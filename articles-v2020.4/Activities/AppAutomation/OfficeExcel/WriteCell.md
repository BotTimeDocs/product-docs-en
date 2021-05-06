# Write Cell

Use the activity to write data into a specified cell of an Excel file.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When Yes is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when No is selected, if there is an error during the execution of the activity, the flow will stop and throw an error
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Data**: The data written into the cell. Only string variables and strings are supported.
  > You can pass in “the output variable of the read cell” to achieve the copy-paste effect while keeping the formatting of the copied data source.

### Target

- **Cell**: The address of the target cell where the data is written. Cells or regions can be entered. Only string variables and strings are supported. When a region is entered, the same data shall be entered in each cell of the specified region.
- **Worksheet**: The target worksheet where the data is written. Only string variables and strings are supported. If the specified worksheet does not exist, the worksheet shall be created in the Excel file.

## Operation sample

1. Drag the **Open/New** activity into the project flow: 

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/excelopencreate20210506.png)

2. Double-click Open, and click **...** to select the local Excel file: 

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/doubleclickopen20210506.png)

3. Drag the **Read Cell** activity into the project flow, enter the sheet name, enter the cell name, and create a new variable "cellContent" of the type String to store the cell contents:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/readcell20210506.png)

4. Drag the **Write Cell** activity into the project flow, and enter the sheet name, cell name, and the variable to be written. "cellContent" is used here. That is, the contents of A1 are written to A2:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/writecella220210506.png)

5. Click Run. After the running is successful, open Excel to check if the contents of A1 have been written to A2: 

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/runningresult20210506.png)
