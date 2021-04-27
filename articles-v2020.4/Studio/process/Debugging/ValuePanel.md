# Variables Panel

The **variables panel** is mainly used to display the values of user-defined variables and activity properties. The details are as follows.

- Global Variable
- Input/output properties of the previous activity

This panel is visible only during the debugging process. The variables and properties in the variables panel can be expanded/collapsed, which is useful for displaying complex types of variables.

![Variables Panel](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/variablePanel.PNG)

Using this panel, we can clearly see the type and value of each variable in the current activity. When the running flow is paused at the breakpoint, the next step debugging starts. At this time, you need to pay special attention to observe whether the data of each step of the flow is correct so as to determine whether the flow is executed correctly.</br> If the data error occurs or the flow does not enter the pre-set breakpoint when the flow runs, you need to re-determine the location of the flow error according to the error message and running logic, reset the breakpoint, and continuously refine the flow to find the error location of the flow.

For the value of a property, when the length of the value exceeds the limit, it will be truncated and not displayed in its entirety.</br> At this point, the mouse hovers over the area where the value is located and clicks on it to open the "View Value" floating window. The window can be resized by dragging the bottom right corner to display the full value information.</br> If you need to copy out the value information, just click Copy in the upper right corner of the "View Values" floating window.

![Debugging - View Values](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Debugging/debugging-view.PNG)