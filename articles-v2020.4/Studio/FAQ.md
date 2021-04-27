# FAQ

## Installation

1. **Q: A program crash prompt pops up during the installation, as shown in the following figure:**
   
   ![Installation crash](https://docimages.blob.core.chinacloudapi.cn/images/Studio/FAQ/installCollapse.png)
   
   **A:** Choose Control Panel > Programs > Uninstall a program to display the list of currently installed programs. Check whether .Net Framework has been installed, such as .Net Framework 4.6.1 or later. If .Net Framework is not installed, download and install .Net Framework 4.6.1 first. Then restart the computer and install ENCOO RPA Studio. Download URL:<https://www.microsoft.com/zh-CN/download/details.aspx?id=49982>

2. **Q: A installation failure message is displayed after I click Install.**
   
   **A:** Check the read and write permissions of the current user for the installation directory. If the current user has not been granted the read and write permissions for the installation directory, you need to log in as an administrator. Right-click the installation directory and click Properties. Click the Security tab, add the target user account, grant full control permissions to this user, and click OK. Then log out and relog in as the target user to try the installation again.

3. **Q: What is the default installation directory of the Studio?**
   
   **A:** `%UserProfile%\AppData\Local\Encoo Studio`

4. **Q: What is the default installation directory of the Robot?**
   
   **A:** `%programfiles(x86)%\Encoo Robot`

## Uninstallation

1. **Q: Uninstallation failed.**
   
   **A:** </br> (1) Delete the encootech folder under the installation directory. The installation directory is under the Program Files (x86) directory. The installation directory of a version later than 25 is under AppData\\Local\\ in your user folder. </br> (2) In C:\\ProgramData\\Package Cache\\, search for all folders with names starting with Digi4th and delete all these folders. </br> (3) Use the command sc delete DataBusService to delete the Windows service DataBusService.

## System Logs

1. **Q: What is the default system log path of the Studio and Robot?**
   
   **A:** `%UserProfile%\AppData\Local\Encoo\Log`.

2. **Q: What is the default installation log path of the Studio and Robot?**
   
   **A:** `%UserProfile%\AppData\Local\Encoo\Installation`.

## Market

1. **Q: What is the path on the local computer for storing activity packages installed from the activity market?**
   
   **A:** `%UserProfile%\.nuget\packages`

## Plug-ins

1. **Q: Chrome screen recording failed. What are the causes of automation failure?**
   
    **A:** </br> 
    (1) Check whether the Chrome brower extension has been installed. Check whether the Chrome plug-in has been installed and enabled, as shown in the following figure:
   
    ![Enable the extension](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Extensions/chrome-usingExtension.png)</br>

    (2) After Chrome opens, check whether the process EncooNativeMessageHost.exe exists in the job manager. This process is a communication process between RPA and Chrome. Perform the checks in (1) if the process is not found.
   
    ![Check the process](https://docimages.blob.core.chinacloudapi.cn/images/Studio/FAQ/taskManager.png)</br>

2. **Q: How to install the Chrome plug-in?**
   
    **A:** Open the Studio, choose **Start > Tools > Extension**, click "Chrome Extension", and then follow the wizard to complete the installation. After the installation is complete, open the Chrome browser manually and enter chrome://extensions/ to enable the extension.
   
    ![Install Extension](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Market/extensioninpath20201019.png)