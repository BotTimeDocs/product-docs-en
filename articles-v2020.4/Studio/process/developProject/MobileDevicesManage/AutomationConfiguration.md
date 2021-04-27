# Step 3: Automated service configuration

## Android

### Connect Service

1. Decompress the downloaded mobile service pack **Encoo.Android.Automation.zip**.
   
    > **Description:**
    > 
    > You need to make sure that the decompression path does not contain Chinese characters.

2. In the decompressed folder, double-click on the application **Encoo.Android.Automation.exe**.

3. In the **ENCOO Android Service Manager** dialog box, click **Connect Service**.
   
    ![Android Connect Service](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Andriodconnect20201104.png)

4. The service connection is successful, as shown in the following figure.
   
    ![Successful Service Connection](https://docimages.blob.core.chinacloudapi.cn/images/Studio/serverconnectsucess20201104.png)

### Install Application (for the first time)

In the **apk** folder under the decompressed folder, there are three mobile application installation packages as follows.

![Application](https://docimages.blob.core.chinacloudapi.cn/images/Studio/app20201104.png)

> **Description:**
> 
> - "pocoservice-debug" and "Yosemite" are installed by default by the system itself, so users do not need to install them manually.
> - "SmsObserver" is used for the "Receive SMS Verification Code" activity. It should be installed by users as needed.

| **No.**| **Installation Package**| **Description**
|----------|----------|----------
| 1| pocoservice-debug| It is used to display information about element controls on the mobile page.
| 2| SmsObserver| It is used in conjunction with the **Receive SMS Verification Code** activity to receive the SMS verification code.<br> **Description**: <br> - This application supports Android 6.0 and above. <br> - The "Read SMS Content" permission needs to be set to "Allowed".
| 3| Yosemite| The default input method used during the test can be manually modified after the test.

## IOS

### Connect Service

Perform the following operations on a **Mac computer**.

1. Decompress the downloaded mobile service pack **Encoo.IOS.Automation.zip**.
   
    > **Description:**
    > 
    > You need to make sure that the decompression path  does not contain Chinese characters.

2. In the decompressed folder, double-click on the application **EncooIOSAutomation**.
   
    > **Description:**
    > 
    > - The first time you run the app, you may need to enable the Allow option in "Settings > Security \& Privacy" on your Mac.
    > - If "The file is corrupted" is displayed when you double-click the application, refer to the [Solutions](https://www.macdo.cn/925.html).

3. In the **ENCOO iOS Service Manager** dialog box, click **Connect Service**.
   
    ![iOS Connect Service](https://docimages.blob.core.chinacloudapi.cn/images/Studio/iosconnect20201104.png)

> **Description:** When you connect the phone after the service is enabled, the following problems may be encountered for reference.
> - Problem 1: xcode-select: error: tool ‘instruments’requires Xcode or relevant log status output when the connection is displayed in the IDE. <br> Solution reference: <br> - View the path where Xcode is installed (find Xcode and drag it directly to the terminal to view the path) <br> - Execute the command sudo xcode-select --switch the Xcode path /Contents/Developer/ displayed in the terminal
> - Problem 2: IDE can't connect to the phone. <br> Solution: Check whether python is already installed in the /usr/bin folder. If so, you need to uninstall the old python version first.