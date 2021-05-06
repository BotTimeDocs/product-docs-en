# License List

On the "Global Management" - "License" page, you can view the information of licenses authorized within the active tenant. You can click the "View Usage" button to view detailed usage information for each type of license.

![License](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4License1.png)

## Using Studio License

When you log in to your studio using the console account, the corresponding version of the studio license on the license page will be used: After login, the usage quantity is displayed as +1 for the Studio Enterprise Edition licence. You can also view the active user and device name in the "View Usage" list.

![License](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4License2.png)

The "Preemptive" strategy applies for studio quotas of the console. All accounts under the tenant can log in to the license used by the studio.

## Releasing Studio License

You can release some used studio licenses for being used by others by either of the following methods:

1. Locate an icon in the upper right corner of your studio, and click **Logoff**. After logoff, the studio quota used by the device is immediately released.
2. On the "Global Management" - "License" page, click "**View Usage**", locate the quota you want to release, and click "**Remove License**". The used studio quota is immediately released. The related studio will be logged off next time the license is verified.

## Using Robot License

When you add a robot in the console, a new robot will use a corresponding type of robot quota on the license page. For example, when you add a robot Enterprise Advanced Edition in the console, the usage quantity is displayed as +1 for the Robot Enterprise Advanced Edition licence.

![License](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4License3.png)

When used quotas reach the license limit, no new robot can be added and robots already added can works normally.

## Releasing Robot License

You can release some used studio licenses for being used by others by either of the following methods:

1. On the "Robot Management" page, select the robot to release the license, and click the "**Remove License**" button. The license authorized to the robot is removed.
2. On the "Global Management" - "License" page, click "**View Usage**", locate the quota you want to release, and click "**Remove License**". The license authorized to the robot is removed.

## Document Understanding Service License

The document understanding service license is mainly used to control the number of times the document understanding template can be invoked. At present, it is controlled according to the built-in model type.

![License](https://docimages.blob.core.chinacloudapi.cn/images/Console/ConsoleAdmin/EnV4License4.png)