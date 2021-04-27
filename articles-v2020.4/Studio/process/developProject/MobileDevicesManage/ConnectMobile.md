# Step 2: Connect your phone

When developing mobile client software, you usually can debug your application by using an emulator or a real device. Both ways will be introduced here, and you can choose according to your needs during the actual operation.

> **Note:**
> 
> If you have opened a security software such as "360 Security Assistant" on your PC, please close it before the service is started.

## Android

### Prerequisites

Add ADB environment variables.

> **Description:** ADB is the official Android debugging tool provided by Google.

<br> Create ADB system environment variables (The address of ADB system environment variables is configured according to the path of the unpacked file of the mobile service pack Encoo.Android.Automation.zip) and add it to Path in the format: "(**PC File Path**)\\Encoo. Automation\\airtest\\core\\android\\static\\adb\\windows", where the content in brackets changes according to the actual situation and the rest remains the same. such as: `D:\workspace\Encoo\Encoo.Android.Automation\airtest\core\android\static\adb\windows`

![Environment Variables](https://docimages.blob.core.chinacloudapi.cn/images/Studio/environment20201104.png)

> **Description:**
> 
> - If other ADB environment variables are already configured in the system environment variables (such as emulator), you need to delete the configuration of the corresponding ADB environment variables.
> - If the service path changes every time you update the Android service pack, you need to reconfigure the ADB environment variables.

### Way one: Android emulator

**Android emulator** is an emulator that can run and simulate the Android mobile system and install, use and uninstall Android applications on a personal computer. With the Android emulator, users can use mobile applications in the emulator even without a mobile hardware device.

1. There are many types of emulators for testing or using APP, such as MuMu, MEmu Play, NoxPlayer. You can download and install the Android emulator on your PC according to your needs.
   
    ![Android Emulator](https://docimages.blob.core.chinacloudapi.cn/images/Studio/androidmonitor20201104.png)

2. It is similar to the phone. You need to enable **Developer Options - Allow USB Debugging** in the emulator.
   
    ![Developer Options](https://docimages.blob.core.chinacloudapi.cn/images/Studio/developeroption20201104.png)
   
    > **Description:**
    > 
    > For mainstream emulators, refer to the following table.
   
    | **No.**| **Emulator Name**| **ADB Connection Code**
    |----------|----------|----------
    | 1| NetEase MuMu| adb connect 127.0.0.1: 7555
    | 2| NoxPlayer| adb connect 127.0.0.1: 62001
    | 3| MEmu Play| adb connect 127.0.0.1: 21503
    | 4| iTools| adb connect 127.0.0.1: 54001
    | 5| TianTian| adb connect 127.0.0.1: 6555
    | 6| Droid4X| adb connect 127.0.0.1: 26744
    | 7| BlueStacks| adb connect 127.0.0.1: 5555


3. In the **Command Line Prompt** interface on the PC, connect the Android terminal device to the PC via the ADB connection code of the corresponding emulator.
   
    ![Command Line Prompt](https://docimages.blob.core.chinacloudapi.cn/images/Studio/cmd20201104.png)

### Way 2: Connect a real Android device over USB

The mobile phone system versions from Android 4.4 to Android 10 are currently supported, with the exception of MIUI 11 and MIUI 12 based on Android 9 and Android 10, respectively.

1. The real Android device is connected to the PC with a USB cable.

2. Enable Developer Mode
   
   There may be differences in the way of enabling the developer mode on every phone, so if you don't know how to enable the developer mode on your own phone, you can search for "how to enable developer mode on xxx model phone" on Baidu.
   
   > **Description:**
   > 
   > - After enabling the developer mode, you need to check the **USB Debugging** box in the **Developer Options**.
   > - For some phones, "**Allow Location Simulation**" and "**Allow Application Installation via USB**" should be enabled.

3. Connect to a Computer
   
   When connecting to a computer, you may need to install the phone's drivers so that the computer can recognize and unlock the phone.
   
   > **Description:** In general, when the data cable is connected to the USB port on the PC, the phone driver will be installed automatically, unless a prompt such as "Driver installation failed" pops up on the PC, then you need to install it manually.

4. Connection Test
   
   In the **Command Line Prompt** interface on the PC, enter the command `adb devices`. An example of a successful connection is shown as follows:
   
   ![Example of Successful Connection](https://docimages.blob.core.chinacloudapi.cn/images/Studio/deviceconnect20210129.png)
   
   > **Description:**
   > 
   > In case of an unsuccessful connection, the following can be referred to.
   > 
   > - If you are prompted that **adb is not recognized as an internal or external command**, please check if you have configured adb system environment variables.
   > - If you do not see the **Device Number device** line, you need to check whether the computer has installed the corresponding official driver software for the phone. If the driver has not been installed, the phone can not be detected. Please visit the official website of the device manufacturer to download and install the official driver.
   > - It is recommended to use the USB port on the back of the computer case as much as possible. The USB port on the front of the computer may be less stable.
   > - You need to enable the Developer Options and USB Debugging option on the phone, and select Allow the PC to debug the device when the device is connected to the computer, otherwise, the phone status is **unauthorized**, indicating that it cannot be connected.
   > - You need to make sure that all phone assistant software on your computer is closed and ADB processes are fully exited (Most phone assistants need to be manually terminated in job Manager).

## IOS

Xcode is an integrated development environment (IDE) running on Mac OS X. It comes with an emulator for each model of iphone/ipad/iwatch/itv. The emulator is used for development debugging and no apps from the App Store can be installed on it.

Perform the following operations on a **Mac computer**.

> **Description:**
> 
> When the Mac computer is connected to the phone: It is recommended that the phone's **Lock Screen** (Phone Settings - Display \& Brightness - Auto-Lock) be set to **Never** to prevent the phone from locking the screen during recording or playback and causing operation failure.

1. Download the development and debugging tool Xcode version 11.1.
   
   Download link: `https://developer.apple.com/download/more`
   
    ![Install Xcode](https://docimages.blob.core.chinacloudapi.cn/images/Studio/installxcode20201104.png)
   
    > **Description:**
    > 
    > - If the phone system version is iOS 13.0 or above (iOS 14.0 or above is not supported at this time), you need to put the unpacked debug package of the corresponding version into the path /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS. platform/DeviceSupport and restart Xcode.
    > - Download link for each version of debug package: `https://pan.baidu.com/s/1O9x8-wE0UIsA7GLWdLrMkw`  Password: `refx`

2. Install Dependencies
   
    Perform the following installation operations in the Mac PC terminal.
   
    a. **Install brew**
   
    brew is a package manager for macOS. It can simplify the installation of software on macOS and Linux operating systems.
   
    step1：Enter the installation command:
   
    ```bash
    /usr/bin/ruby -e "$(curl -fsSL https://hellogithub.cn-bj.ufileos.com/file/ brew_install.sh)"
    ```
   
   OR
   
    ```bash
   
    /usr/bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)" 
    ```
   
    step2: Check whether the installation is successful.
    
    ```bash
    brew --version
    ```
   
    > **Description:**
    > 
    > During the operation, the following issues may be encountered for reference.
    > 
    > - Issue 1: Homebrew installation error `curl : (7) Failed to connect to raw.githubusercontent.com port 443: Operation` Solution reference: `https://www.jianshu.com/p/dea776e7effb` or `https://blog.csdn.net/heroacool/article/details/102844367`
    > - Issue 2: `/usr/bin/zsh：No such file or directory` Solution reference: `brew install zsh https://www.cnblogs.com/mafeng/p/10569559.html`
    > - Issue 3: brew installation timeout, slow speed Solution reference: `https://www.jianshu.com/p/6b486e12454f`
   
    b. **brew install usbmuxd**
   
    > **Description:**
    > 
    > During the operation, the following issues may be encountered for reference.
    > 
    > - Issue 1: local permissions issue Solution reference: `https://www.cnblogs.com/tinys-top/p/12299663.html`
   
    c. **brew install libimobiledevice**
   
    d. **brew install ideviceinstaller**

3. Obtain Real Device UDID
   
    UDID (Unique Device Identifier) is a sequence of 40 letters and numbers that uniquely identifies an iOS device, including iPhones, iPads, and iPod Touches.
   
    In Xcode Tools, select **Window - Devices** to view the device identifier, copy and paste it, and contact the developer (ENCOO developer) to configure a debuggable certificate.
   
    ![Obtain Real Device UDID](https://docimages.blob.core.chinacloudapi.cn/images/Studio/getudid20201104.png)
   
    > **Description:**
    > 
    > Xcode comes with an emulator interface as shown below.
   
    ![iOS Emulator](https://docimages.blob.core.chinacloudapi.cn/images/Studio/iosmonitor20201104.png)

4. Download the configured certificate to the Xcode Tools

a. Open Xcode Tools

![Xcode Icon](https://docimages.blob.core.chinacloudapi.cn/images/Studio/xcodeicon20201104.png)

b. Open **Xcode Preferences > Accounts**, click the "+" in the bottom left corner of the screen, enter your Apple ID (Developer) and password, and save.

![Xcode Account Configuration](https://docimages.blob.core.chinacloudapi.cn/images/Studio/xcodeaccount20201104.png)

c. After selecting the configured certificate, click **Download Manual Profiles** to download it.

![Download Certificate](https://docimages.blob.core.chinacloudapi.cn/images/Studio/downloadprofiles20201104.png)