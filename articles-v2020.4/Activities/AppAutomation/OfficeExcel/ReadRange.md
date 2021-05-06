# Read Range

Get the cell range data in the workbook and store it in the data table variable. If the cell range is not specified, read the data in the whole table by default. (Read “rows, columns, ranges, worksheets” through variable connection input)

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When Yes is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when No is selected, if there is an error during the execution of the activity, the flow will stop and throw an error
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **Worksheet**: The worksheet where the target cell range is located. Only string variables and strings are supported
- **Range**: The target cell range for reading data. If the cell range is not specified, read the data in the whole table by default. Only string variables and strings are supported

### Output

- **Data**: Store the read data in the target range in this variable. Only data table variables are supported

### Option

- **Retain format**: When the option is checked, the data content and data format (such as currency, date) of the target cell range will be read simultaneously, and this data format will be retained as an input of “write range”. When the option is unchecked, the default “regular” data format will be used in “write range”.
- **Use filter**: When the option is checked, the data beyond the filtering range in the specified area will not be read. When the option is unchecked, all data in the specified area will be read at the same time, including the data beyond the filtering range.
- **Add column header**: When the option is checked, the first row of the worksheet will be the column header of the newly generated data table. When the option is unchecked, the default column header of the newly generated data table is “1, 2, 3...”

## Operation sample

1. Drag the **Open/New** activity into the project flow:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/excelopencreate20210506.png)

2. Double-click Open, and click **...** to select the local Excel file:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/doubleclickopen20210506.png)

3. Drag the **Read Range** activity to the project flow and fill in the sheet name "sheet1". Fill in the read range "A1:D3" and create a new variable "datatable" of type datatable", which is used to store the contents of all cells in the region. 

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/dragthereadrange20210506.png)

4. Drag the **Write Range** activity into the project flow, fill in the sheet name "sheet2", and fill in the write range "A1:D3". Fill in the variables to be written, and here "datatable" is used. That is, the contents of "A1: D3" in "sheet1" are written into "A1: D3" in "sheet2".

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/dragwriterange20210506.png)

5. Click Run. After the running is successful, Open Excel to see that the contents of the "A1:D3" in the range of sheet1 have been written into "A1:D3" in sheet2.

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/runresult20210506.png)