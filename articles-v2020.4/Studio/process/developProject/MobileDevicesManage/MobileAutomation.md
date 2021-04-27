# Step 5: Mobile automation operations

As with interface automation on the PC, ENCOO RPA provides a number of mobile automation activities for mobile automation, which can obtain the elements on the phone.

> **Description:**
> 
> The following operations are performed on the PC of the Windows operating system for both Android and iOS mobile devices.

## Operation example

Take turning off mobile data on a phone as an example.

1. Drag a **Connect Device** activity into the flow.
   
    ![Connect Device](https://docimages.blob.core.chinacloudapi.cn/images/Studio/connectdevices20201104.png)

2. In the **Mobile Device Manager** panel, click the "Copy Device Information" option.
   
    ![Copy Device Information](https://docimages.blob.core.chinacloudapi.cn/images/Studio/copydevices20201104.png)

3. Double-click on the **Connect Device** activity in the flow screen and click on "Autofill in One Click" to automatically fill in the information for the connected device.
   
    ![Connect Device](https://docimages.blob.core.chinacloudapi.cn/images/Studio/connectdevicesfullin20201104.png)

4. In the "Mobile Device Manager" panel, click the "Record" button in the "Smart Recorder" on the right side to record.
   
    ![Smart Recording](https://docimages.blob.core.chinacloudapi.cn/images/Studio/recoder20201104.png)
   
    > **Description:**
    > 
    > For operations of the Smart Recorder, see [Smart  Recording](Studio/process/../../../Recording/Recording.md).

5. For the recorded flow, after you click the "Save" button, a sequence will automatically be generated in the "**Connect Device**" activity.
   
    ![Flow Recording Completed](https://docimages.blob.core.chinacloudapi.cn/images/Studio/flowdone20201104.png)

6. Click the "Run" button in the **run panel** to run the flow.
   
    ![Run](https://docimages.blob.core.chinacloudapi.cn/images/Studio/run20201104.png)

</br> A separate mobile phone interface will pop up in the running flow to simulate the effect of manually operating the phone.

![Running Process Interface](https://docimages.blob.core.chinacloudapi.cn/images/Studio/runprocessUI20201104.png)