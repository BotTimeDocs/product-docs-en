# Java Extension

**Java Extension** is applicable to the automation of Java1.6 or higher applications.

> **Description:**
> 
> For applications opened with Java 9+ JRE:
> 
> - Prior to Java 9, JRE included the attach module, which Java Extension relies on to automate Java applications.
> - For Java 9+, the attach module is only included in JDK. For applications opened with JRE9+, you need to manually add this module under JRE directory.

## Install from Studio

1. **Close all Java applications**, click the Tools icon on the left toolbar of Studio.

2. Choose Extensions > Java Extension, and a confirmation window appears.

3. Click OK, to launch the installer of Java extension as administrator. Click Yes on the User Account Control window to start the installation.

4. After the installation is successful, you will be prompted that the Java Extension installation is successful.
   
   > **Description:**
   > 
   > When you try to record an application that does not have the Java plug-in installed and cannot be automatically injected, Studio will also guide you to install the Java plug-in. At this point the Java plug-in will only be installed into the JRE of the currently recorded application.

## Install from the Command Line

1. **Close all Java applications,** find the extension installer EncooJavaExtensionInstaller.exe in the JavaSupport folder under the Studio installation directory.
   
   > **Description:**
   > 
   > The installation directories for different versions can be found as follows:
   > 
   > - Installation directory for the versions prior to 1.1.2009.X: `C:\Users\UserName\AppData\Local\Encoo\Encoo Studio\IDE\JavaSupport`, where `UserName` is the actual user name.
   > - Installation directory for version 1.1.2009.X and later: C:\\Users\\UserName\\AppData\\Local\\Encoo Studio\\app-x.x.xxxx.xx\\Extensions\\Java, where UserName is the actual user name.

2. Open the command line as administrator, and switch to the installation directory path of corresponding version, e.g., `cd C:\Users\UserName\AppData\Local\Encoo Studio\app-x.x.xxxx.xx\Extensions\Java`

3. Execute the installation command: `EncooJavaExtensionInstaller.exe -install -a`

## Manual Installation

In addition to automatic installation, we still support manual installation for situations where automatic installation does not work.

1. Find the JavaSupport folder under the Studio or Robot installation directory.
   
   ![img](https://docimages.blob.core.chinacloudapi.cn/images/Amanda/Java/1.png)
   
   > **Description:**
   > 
   > For version 1.1.2009.X and later, it is the Extensions\\Java folder under the installation directory.

2. For Studio of version 1.1.2009.X and later, copy accessibility.properties in the JavaSupport folder to the \\lib directory of runtime, copy BotTimeJavaBridge.jar in the JavaSupport folder to \\lib\\ext directory of runtime, and then copy `BotTimeJavaBridge-*.dll` and `BotTimeJAWTBridge-*.dll` to the `\bin\ in runtime`. (Copy the dll with the appropriate suffix depending on whether the runtime is 32-bit or 64-bit)
   
   | Extension File| Destination Path
   |----------|----------
   | BotTimeJavaBridge-32/64.dll| %JAVAHOME%\\bin
   | BotTimeJAWTBridge-32/64.dll| %JAVAHOME%\\bin
   | accessibility.properties| %JAVAHOME%\\lib
   | BotTimeJavaBridge.jar| %JAVAHOME%\\lib\\ext
   | jaccess.jar| %JAVAHOME%\\lib\\ext



## EncooJavaExtensionInstaller Tool

**EncooJavaExtensionInstaller** is an application used to automatically deploy Java extensions on your computer. It supports full disk scan or installing/uninstalling Java plug-ins in specified directories.

> **Note:**
> 
> - It is recommended to run as administrator to avoid permission issues during installation.
> - It is recommended to close any Java applications before installation or uninstallation to avoid file hogging problems.

### Install

- EncooJavaExtensionInstaller.exe -install -a, fully scan JRE and install the Java plug-in, this operation may take a long time.
- EncooJavaExtensionInstaller.exe -install -d, scan the default location (Program Files \&\& Program Files (x86)) for public JRE and install the Java plug-in.
- EncooJavaExtensionInstaller.exe -install -p "specified path", install the Java plug-in to a specified path, the path can be the path or the directory where the java.exe or javaw.exe is located.

### Uninstall

- EncooJavaExtensionInstaller.exe -uninstall -a, fully scan JRE and uninstall the installed Java plug-in, this operation may take a long time.
- EncooJavaExtensionInstaller.exe -uninstall -d, scan the default location (Program Files \&\& Program Files (x86)) for public JRE and uninstall the installed Java plug-in.
- EncooJavaExtensionInstaller.exe -uninstall -p "specified path", uninstall the Java plug-in that is installed to a specified path, the path can be the path or the directory where the java.exe or javaw.exe is located.

## FAQ

1. **"Could not find 32-bit/64-bit Java runtime environment" is prompted**
   
   Encoo could not find the public Java runtime environment to initialize Java extensions, you need to install 32-bit or 64-bit JRE as prompts. The corresponding version of Java can be downloaded from the following address:<https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html>
   
   a) Click Accept License Argument
   
   ![Accept License Argument](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Extensions/java-acceptLicenseArguments.png)
   
   b) Click and download 32-bit or 64-bit Java (32-bit for x86, 64-bit for x64) according to the Encoo prompts
   
   ![Download Java](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Extensions/java-downloadJava.png)

2. **For Java Applet applications or applications that cannot attach, you need to manually install Java extensions to the runtime directory**
   
   a) Find the JavaSupport folder under the Studio or Robot installation directory
   
   ![Look for JavaSupport folder](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Extensions/java-javaSupport.png)
   
   > **Description:**
   > 
   > For Robot of version 1.1.2010.17 and later, it is the Extensions\\Java folder under the installation directory.
   
   b) For Robot of version 1.1.2010.17 and later, copy accessibility.properties in the JavaSupport folder to the \\lib directory of runtime, copy BotTimeJavaBridge.jar in the JavaSupport folder to \\lib\\ext directory of runtime, and then copy `BotTimeJavaBridge-*.dll` and `BotTimeJAWTBridge-*.dll` to the \\bin\\ directory of runtime. (Copy the dll with the appropriate suffix depending on whether the runtime is 32-bit or 64-bit)