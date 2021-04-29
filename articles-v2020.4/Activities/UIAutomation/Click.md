# Click

Simulate mouse clicking operation. Desktop and browser elements are supported. Also, image recognition of specified elements on the desktop is supported, not on the browser yet

## Property

### Basic

- **Display Name**: It is the name of this activity by default. As change is supported, the user can define the display name of this activity.
- **Proceed After Failure**: Set whether to ignore this error and proceed to the next activity when the execution of this activity failed. Select from the dropdown. When "Yes" is selected, if there is an error during the execution of the activity, the flow will proceed to the next activity and not stop; when "No" is selected, if there is an error during the execution of the activity, the flow will stop and throw an error.
- **Pre-delay (ms)**: Specify the time to wait before this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after the previous activity is executed, this activity will be executed after waiting for one second.
- **Post-delay (ms)**: Specify the delay time after this activity is executed. The unit is ms, 1000 ms = 1 s. If 1000 is entered here, it means that after this activity is executed, the next activity will be executed after waiting for one second.
- **Timeout (ms)**: Specify the execution time of the activity. The unit is ms, 1000 ms = 1 s. It includes matching timeout (ms). If the time limit is exceeded and the activity has not yet been executed, an error will be thrown.

### Target

- **Control element**: Receive the variable as the target element to be clicked. Either this item or the **selector** can be filled in
- **[Selector](../Appendix/Selector.md?_v=v2020.4)**: Indicate the target position to be clicked. It can be generated automatically by clicking on the **specified element**. Only string variables and strings are supported
- **Matching timeout (ms)**: Limit the time to find the target element. No waiting time will be given after the specified time limit is exceeded. If the specified element is not matched after the time limit is exceeded, an error will be thrown. The unit is ms, 1000 ms = 1 s. Only integer variables and integers are supported

### Click

- **Click Type**: Select the type of simulating mouse clicks by the drop-down box. There are four types: click, double click, press, release
- **Cursor position**: Describe the starting point of the cursor to which offsets from the **OffsetX** and **OffsetY** properties are added. The default option is **Center**
- **Mouse button**: Select the button that simulates mouse clicks. For example, when the left button is selected, it will simulate the left button click.
- **OffsetX**: Horizontal displacement of the cursor position according to the option selected in the **Cursor Position** field. For example, if you fill in "10", it means horizontal displacement to the right by 10 pixels from the **Cursor Position**. For screen coordinates, the origin is the upper-left corner of the screen. Only integer variables and integers are supported
- **OffsetY**: Vertical displacement of the cursor position according to the option selected in the **Cursor Position** field. For example, if you fill in "10", it means vertical displacement to the bottom by 10 pixels from the **Cursor Position**. For screen coordinates, the origin is the upper-left corner of the screen. Only integer variables and integers are supported
- **Percentage of horizontal coordinate**: Percentage shift according to the **Cursor Position**. The length of the rectangular box specified by the click is multiplied by the value of this property, and the result is added to the horizontal coordinate of the **Cursor Position** to obtain the final horizontal coordinate of the click. For example, if you fill in "0.5" and select "Center" as the cursor position, the calculation process of the final click position is as follows. Take the length of the rectangular box of the specified element and multiply it by 0.5. The result is half of the length of the rectangular box. Then the result is added to the cursor position "Center". The final number obtained is the horizontal coordinate of the click, which is located at the center of the right side of the rectangular box
- **Percentage of vertical coordinate**: Percentage shift according to the **Cursor Position**. The length of the rectangular box specified by the click is multiplied by the value of this property, and the result is added to the vertical coordinate of the **Cursor Position** to obtain the final vertical coordinate of the click. For example, if you fill in "0.5" and select "Center" as the cursor position, the calculation process of the final click position is as follows. Take the width of the rectangular box of the specified element and multiply it by 0.5. The result is half of the width of the rectangular box. Then the result is added to the cursor position "Center". The final number obtained is the vertical coordinate of the click, which is located at the center of the bottom side of the rectangular box

### Option

- **Click method**: Select the method used to simulate mouse clicks. It includes three values, that is, default, mouse simulation, and control setting. The default value of this property is **Default**. It is implemented to automatically apply the best click method based on the type of element specified by the user (such as desktop or browser). When some scenarios cannot be executed successfully using the default property value, this property value can be manually modified to **Mouse Simulation** or **Control Settings** to adapt to a few special scenarios to make it execute successfully.
- **Auxiliary Key**: It includes: None, Shift, Ctrl, Alt, Win. It allows you to click while pressing an auxiliary key. It only takes effect when the click method is mouse simulation. It does not work for the control setting.

> **Description:**
> 
> - When a desktop element is specified. After the <b>Control Settings</b> is selected as the property of the <b>click method</b>, only <b>left-click</b> is supported. The settings of the <b>cursor position, offsetX (Y), and horizontal (vertical) coordinate percentage</b> are not supported
> - When a browser element is specified. After the <b>Control Settings</b> is selected as the property of the <b>click method</b>, only the JS events supported by the selected element are supported. When there are scenarios that cannot be overwritten, the property value can be changed to <b>Mouse Simulation</b>.

## Operation sample

1. Drag in the **Click** activity and specify the element: ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/Click/Click1.png)

2. Open the selector window and click on the Unverified button to verify whether or not the specified element is recognized: ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/Click/Click2.png)

3. The web page with the element specified in step 1 remains open. Click to run the flow. ![](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/%E7%95%8C%E9%9D%A2%E6%88%AA%E5%9B%BE/Click/Click3.png)

For more types of clicks, please click on the [link](https://academy.encoo.com/learn/unit-detail/33) to view the ENCOO Academy advanced courses.
