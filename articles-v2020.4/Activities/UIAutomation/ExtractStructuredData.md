# Get Structured Data

Get structured data for a specified page, and the page can be automatically turned for more data. The whole table data or single column data in the table and the custom property information of the data are available. During runtime, take the data within the specified maximum number of extracted items. Desktop and browser are supported.

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.

### Target

- **XML data**: Define what types of data are extracted from the web page. XML is automatically generated after "Specify Data Source".
- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Indicate the target area where the data is to be acquired. It can be generated automatically by clicking on the **Specified Data Source**. Only string variables and strings are supported
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Option

- **The maximum number of extracted items**: the maximum number of data items to be acquired. For example, if this value is entered as "10", the maximum number of data items in the data table returned at runtime will be 10. Only integer variables and integers are supported
- **Next page**: Indicate the position of the Next Page button to achieve the function of turning the page to get data. It can be generated automatically by specifying the Next Page button during the process of **Specify Data Source**. Only string variables and strings are supported
- **Delay in getting next page data**: Limit the time to get the new page data after turning the page. After the specified time limit is exceeded, the operation of getting data will be executed. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Output

- **Data table**: Store the obtained structured data into this variable.

## Operation sample

1. Open a web page containing structured data (such as http://news.baidu.com), and drag in the **Get Structured Data** activity. Click Specify Data Source and specify the first element. Then a "Wizard" dialog box will pop up to prompt you to specify the second element of the data source, as shown below.
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-1.png)

2. Specify the second element, and the Wizard dialog box will show the default text column name. Then click the "Next" button, and the "Wizard" dialog box shows all the data obtained and the default maximum number of extracted items: 50:
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-2.png)
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-3.png)

3. Add data table variables and click the "OK" button.
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-4.png)

4. Click "Yes" or "No" as needed. If you select "Yes", continue to select the element on the application page. If you select "No", the process of specifying elements ends
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-5.png)

5. Drag in the **Preview Data Table** activity and enter the data table variable dt defined in the above operation:
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-6.png)

6. Click Run Flow to view the acquired data, as shown below.
   
    ![](https://docimages.blob.core.chinacloudapi.cn/images/Activities/extractStructureData-7.png)