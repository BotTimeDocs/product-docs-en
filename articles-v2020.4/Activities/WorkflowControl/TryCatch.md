# Try Catch

For exception handling, it can catch a specified exception type in a flowchart or activity, and either displays an error notification or dismisses it and continues the execution. It consists of three main sections:

- **Try**: The activity performed which has a chance of throwing an error
- **Catches**: The activity to be performed when an error occurs
  - **Exception**: The exception type to look for. Multiple exceptions can be added
- **Finally**: The activity to be performed after the Try and Catches blocks are executed

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

## Operation sample

1. Drag in the **Open Browser** activity and enter the URL “https://www.aliyun.com”.

2. Set a variable list with the variable type `List<String>` and the default value is new `new List<String>{"Latest Activities", "Products", "Solutions"}`, as shown below.

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/aliyun20210506.png)

3. Drag in the **For Each** activity and set the variable list as the loop body. Drag in the **Try Catch** activity.

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/foreach20210506.png)

4. Double click to open the error catch activity and drag in the **Click** activity to the tryCatch container. Click the "Latest Activity" element at the top of the specified page and open the selector to replace the Sinfo value "Latest Activity" with the variable "{item}":

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/click20210506.png)

5. Click "Add New Catch" and select System.Exception. Drag in the **Write to Log** activity and fill it out and output `exception.Message + "Switch to Initial Page"`. Drag in the **Navigate** activity and enter the URL "https://www.aliyun.com".

    > **Description:**
    >
    > After you click the first element of the list in the try container, the current page will jump to other pages, causing the loop to fail when clicking other elements of the list. Thus, we set the Jump to Initial Page in the catch to initialize the page so that other elements in the list can be clicked as normal.

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/navigate20210506.png)

6. Run the flow to view the results:

    ![](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/trycatch20210506.png)