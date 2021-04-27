# Immediate Execution Flow

In addition to creating flow jobs at regular intervals via the job schedule, you can also execute flows manually and immediately:

1. Select the flow deployment you want to execute immediately on the "Flow Deployment" page and click the "Execute" button in the "Actions" option.
    
    ![workflow](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow8.png)

2. In the "Flow Execution" dialog box, you can reassign the maximum number of failed attempts and argument values, and click the "Execute" button to generate the corresponding job execution after confirming that there are no errors. You can view the corresponding job execution in "Flow Deployment" - "Job List" again.
   
    ![process](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow9.png)
   
   > **Description:**
   > 
   > - When the execution target of a flow deployment is specifying robot: Each robot will execute the flow once, i.e., N robots are associated, and N flow jobs will be generated.
   > - When the execution target of a flow deployment is specifying queue: The flow will be executed only once, i.e., a flow job is generated and dynamically assigned in the queue.