# Connection Management

Connection management is mainly used by users to create and manage various data connectors and establish connections with various types of external data to facilitate subsequent data operations in applications.

## Prerequisites

Log in to the Enterprise Edition console as an administrator.

## Create a new MySQL data connection

1. On the "**ENCOO RPA Console > Data Center > Connection Management**" page, click the "+ New" button in the upper right corner of the page.

2. In the pop-up "New Connection" dialog box, select "MySQL" and click the "Next" button.
   
   ![Create a new MySQL data connection](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/mysql20210507.png)

3. In the "Configure Connection" pop-up box, configure the MySQL connection.
   
   - **Connection name**: You can customize the name of the newly created MySQL connection.
   - **Environment type**: You can drop down to select production environment or test environment.
   - **Connection method**: You can select "Connect via Configuration" or "Connect via Connection String".
   - **Use SSL connection**: Whether to enable SSL connection.
   
    a. Connect via Configuration
   
    ![Connect via configuration](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/connectviaconfiguration20210507.png)
   
    b. Connect via Connection String
    
    ![Configure MySQL Connection](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/connectviaconnectionstring20210507.png)

4. (Optional) Click the "Test" button to test whether the data connection is successful.

5. Click the "New" button to complete the MySQL data connection.

## Create a new Restful API data connection

1. On the "**ENCOO RPA Console > Data Center > Connection Management**" page, click the "+ New" button in the upper right corner of the page.

2. In the pop-up "New Connection" dialog box, select "Restful API" and click the "Next" button.
   
    ![Create a new Restful API data connection](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/restfulapi20210507.png)

3. In the "Configure Connection" pop-up box, configure the Restful API connection.

   - **Connection name**: You can customize the name of the newly created Restful API connection.
   - **Environment type**: You can drop down to select production environment or test environment.
   - **Base URL address**: Fill in the base URL location address.
   - **Headers**: Fill in the key and value of the headers.
   - **Parameters**: Fill in the key and value of the parameters.

    ![Configure Manage Database](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/configureconnection20210507.png)

4. Click the "New" button to complete the Restful API data connection.

## Follow-up Actions

- **View**: On the "Connection Management" page, click the "View" option in the "Actions" column to view and modify the configuration information and data permissions for the selected data connection.
- **Test**: On the "Connection Management" page, click the "Test" option in the "Actions" column to test whether the current data connection is successful.
- **Delete**: On the "Connection Management" page, click the "Delete" option in the "Actions" column to delete the currently selected data connection.