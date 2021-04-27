# Open/New

Open an Office Excel workbook and provide scope for Excel activity operations. After this activity is executed, the specified workbook and Excel application will be closed (if variables are provided in the “Output” of the Properties panel, they will not be closed at the end of the activity). If the specified file path does not exist, a new Excel file will be created when the “New File” property is selected.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When Yes is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when No is selected, if there is an error during the execution of the activity, the flow will stop and throw an error
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Input

- **File Path**: The full path of the Excel file to be opened or created (relative paths are also supported). Only string variables and strings are supported
- **Password**: The password that is required to open a password-protected workbook. Only string variables and strings are supported

### Option

- **Save As**: Save the workbook as a file after the operation. If the Save As full path provided is the same as the original path, the original workbook is overwritten directly. Only string variables and strings are supported

- **New File**: When this check box is selected, if the workbook is not found under the specified path, a new one is created; when this check box cleared, if the workbook is not found under the specified path, an exception is thrown.

- **Auto Save**: When this check box is selected, the workbook is automatically saved for each change made during the execution of the activity. When this check box is cleared, changes are not saved after the execution of the activity is ended.

- **Read-only**: Open the specified workbook in read-only mode.

- **Visible**: When this check box is selected, the workbook will be operated in the visible state. When this check box is cleared, all operations will be performed in the background and are not visible.

- **Enable Macro**: When this check box is selected, the “Enable Macro” effect of the workbook is achieved.

## Operation sample

1. Drag the **Open/New** activity into the project flow: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenExcel1.png)

2. Double-click Open, and click **...** to select the local Excel file: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/OpenExcel2.png)

3. Drag the **Read Cell** activity into the project flow, enter the sheet name, enter the cell name, and create a new variable "cellContent" of the type String to store the cell contents: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadCell1.png)

4. Drag the **Write Cell** activity into the project flow, and enter the sheet name, cell name, and the variable to be written. "cellContent" is used here. That is, the contents of A1 are written to A2: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadCell2.png)

5. Click Run. After the running is successful, open Excel to check if the contents of A1 have been written to A2: ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadCell3.png)