# Manage Flow Deployment

## New Flow Deployment

1. In the Flow Deployment page, click the "New" button to start:
   
   - Fill in the basic information of the flow deployment, select the corresponding flow package and the flow package version number.
   - Set the maximum number of failed attempts, and the flow will be retried automatically according to this number when it fails to execute.
   - Set the job priority (1-5000): The higher the priority, the earlier the job will be executed
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/%E6%96%B0%E5%BB%BA%E6%B5%81%E7%A8%8B%E9%83%A8%E7%BD%B21.1.png)
   
   - Assign the arguments in the flow package:
     
     - Manually Assign: Fill in the arguments to be assigned
     
     - Import Asset: Click "Import Asset" to assign the prestored asset in the Asset Management page
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/%E6%96%B0%E5%BB%BA%E6%B5%81%E7%A8%8B%E9%83%A8%E7%BD%B2%E7%AC%AC%E4%B8%80%E9%A1%B5%E8%A1%A5%E5%85%85.png)
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/%E6%96%B0%E5%BB%BA%E6%B5%81%E7%A8%8B%E9%83%A8%E7%BD%B2-%E5%AF%BC%E5%85%A5%E8%B5%84%E4%BA%A7.png)

2. Click "Next" to configure robot execution target, select Specify Execution Queue/Specify Execution Robot
   
   - Specify Execution Queue: Select from the queues created under the resource group;
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow3.png)
   
   - Specify Robot Selection: Display all robots under the resource group, check corresponding robot, searching by name and tag is supported
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow4.png)

3. Click "Save" to complete the flow deployment creation, Click \[Save and Set Trigger] to start the quick configuration of cron job. (See "Cron Job Management")

## View Flow Deployment Config Info

Click the "Config" button in Flow Deployment to view the configuration information of flow deployment

![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow5.png)

## Basic Config and Argument Modification

In the "Config" page of Flow Deployment, click the "Edit" button to modify the basic configuration information and argument information, and click the "Save" button after the modification is completed.

![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow6.png)

## Delete Flow Deployment

Click the "Delete" button in the selected flow deployment action options to delete corresponding flow deployment.

![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow7.png)