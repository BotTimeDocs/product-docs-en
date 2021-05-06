# View Job Records

## View Job Records List

Go to the Job Records page to view the execution conditions of the flow jobs triggered by all flow deployments by any means.

![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/taskhistory20210506.png)

## Job and Runinstance Description

- **Job**: The flow job created by job schedule or manual execution method that needs to be completed.
- **Runinstance**: The flow job will create specific runinstance to complete the job, and a single job may create several runinstances.

For example, after a job is created, a specific runinstance will be generated to complete the job. If the first execution fails and the retry on failure mechanism is configured, the job will automatically create another runinstance to retry on failure.

## State Description

**Job**:

- Waiting: Waiting for assigning robot to execute the job
- Assigned: A robot has been assigned to execute the job (runinstance has been created)
- Running: The robot is executing the job
- Successful: The job is successful
- Failed: The job is failed
- Canceled: The job is canceled

**Runinstance**:

- Created: The runinstance has been created
- Run: The runinstance is running
- Failed: The runinstance is failed
- Successful: The runinstance is successful
- Canceled: The runinstance is canceled

## View Runinstances under a job

Click the "Expand" button under a job to expand corresponding runinstance list. Three items will be displayed by default. If there are more than three items, click "Expand More" to expand all items. The runinstance mainly includes active robot, start time, end time, and status.

![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/viewruninstances20210506.png)

## Viewing Job Details

Click the "View" button under a job to view the execution details of the job. Job details mainly include the basic execution information and parameter information.

![process](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/viewingjobdetails20210506.png)

## Viewing Log Details

You can view the execution log of a job on the robot in either of the following methods:

1. In the Job List page, click the Log button of a specific runinstance under the job to view the specific execution log of the job on the robot.

    ![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/viewinglogdetails20210506.png)

2. You can also click the View Log button in the Job Details page to view the specific execution log of the job on the robot.

    > **Description:**
    > 
    > The log mainly contains log time, log type, log content, and log screenshot. You can check the "Log Switching" in the upper left corner to quickly switch to the execution log of the job on other robots.
   
    ![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/viewlogbutton20210506.png)

## Terminate Job

To abort a job when it is not completed yet, click the "Abort" button to abort it.

- When a job is terminated, if it has not been assigned to a robot, the job will be terminated directly.
- When a job is terminated, if it has been assigned to a robot and is being executed, a command is sent to the robot to terminate the job and the current job will be failed.

![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/cancel20210506.png)

## Adjust Job Priority

Jobs in the scheduling queue will be executed according to priority (0-5000), and the job with the highest priority will be executed first. If you want to give the priority to a job, click the "Adjust Priority" button for that job to adjust the priority.

![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/adjustpriority20210506.png)

You can enter the corresponding priority number, and the job with the highest number will be executed first.

![job](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/prioritynumber20210506.png)