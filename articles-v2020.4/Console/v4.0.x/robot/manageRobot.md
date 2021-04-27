# View Robot List

Enter **Robot Management** and you can see all the robots in the current resource group. You can choose to switch the **Resource Group** to view the robots in different resource groups.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E6%9C%BA%E5%99%A8%E4%BA%BA%E4%B8%BB%E9%A1%B5.png)

## Add Robot

Click the New button to open the Add dialog box. Fill in the robot name, tags, notes, and select the robot type, and then click OK to create a new robot.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/addrobot.png)

After a robot is successfully added, the system will automatically copy your robot connection string. You can paste the robot connection string directly to the client robot to complete the activation. For more information, see: [Activate Robot](../../../Robot/license.md)

## View Robot Information

Click on the corresponding robot name to view robot details

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E6%9F%A5%E7%9C%8B%E5%8F%8A%E7%BC%96%E8%BE%91%E6%9C%BA%E5%99%A8%E4%BA%BA%E8%AF%A6%E6%83%85-1.png)

## Edit Robot Information

Click the Edit button on the robot details page to start editing the robot information, and click Save after completion of editing. ![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E6%9F%A5%E7%9C%8B%E5%8F%8A%E7%BC%96%E8%BE%91%E6%9C%BA%E5%99%A8%E4%BA%BA%E8%AF%A6%E6%83%85-2.png)

Click on the corresponding robot name to view robot details

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/editrobot.png)

Click the Edit button on the robot details page to start editing the robot information, and click Save after completion of editing

## Remove License

A newly created robot has a license by default. If the status of the current robot is Licensed, click the Remove License button in the Actions section to remove the license from the current robot.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E7%A7%BB%E9%99%A4%E8%AE%B8%E5%8F%AF%E8%AF%81.png)

## Assign License

A newly created robot has a license by default. If the status of the current robot is Licensed, click the Remove License button in the Actions section to remove the license from the current robot.

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E7%A7%BB%E9%99%A4%E8%AE%B8%E5%8F%AF%E8%AF%81.png)

## Delete Robot

Find the robot you want to delete and check Actions - Other - Delete. Then click Delete to delete the robot. If a robot wants to be deleted successfully, the following conditions shall be met.

- The status of the robot is Disconnected
- The robot is currently in the execution queue module and there are no queues with the status of Waiting and Executing

![robot](https://docimages.blob.core.chinacloudapi.cn/images/Console/robot/robot/%E5%88%A0%E9%99%A4%E6%9C%BA%E5%99%A8%E4%BA%BA.png)