# Job Schedule Management

Job schedule is mainly used for users to freely configure job execution schedule for each time dimension and scheduling robots to execute various flows, thus realizing unified planning and scheduling for flow execution.

## View Job Schedule List

Click the "Job Schedule" button of a flow deployment to toggle through all the job schedules under that flow deployment name.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/viewjobschedulelist20210506.png)

## New Job Plan

**Step 1, fill in the job schedule details configuration**

1\) Basic information: Cron Job name, flow deployment name, flow package name \& version number.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/newjob20210506.png)

2\) Schedule time (timed execution time of jobs):
- By minute
- By hour
- By day
- By week
- By month
- By cron expression

<!--![trigger](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow12.png)-->

For the cron jobs that are executed by cron expressions, if you know cron expressions, you can write them by yourself according to the rules, or generate them through the cron expression generation website provided by ENCOO.

3\) Start time of job schedule, deactivation time of job schedule. Start time: After the start time is reached, the job schedule will take effect; Deactivation time: After the deactivation time is reached, the job schedule will not generate any more jobs.

**Step 2, confirm execution targets and arguments** 1) Queue name/robot name: If the execution method of the flow deployment configuration is queue execution, the queue name and remarks are displayed here; if the execution method of the flow deployment configuration is specifying robot, the specific robot name and status are displayed.

2\) Argument information: Display the argument values in the current flow package, if the flow deployment has modified an argument value then the latest value will be displayed here. At this point, reassignment can be done by manually filling in or importing asset.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow13.png) After the cron job is filled in, click "Save", the cron job will be started or deactivated automatically at the set start/deactivation time.

> **Description:**
> 
> - When the execution target of a flow deployment is specifying robot: Each robot will execute the flow once each time the job schedule is triggered. That is, N robots are associated, and N flow jobs will be generated each time the job schedule is triggered.
> - When the execution target of a flow deployment is specifying queue: The flow will be executed only once each time the job schedule is triggered, i.e., a flow job is generated and dynamically assigned in the queue.

## View and Edit Job Schedule Details

Click the "View" button of a job schedule to view the details of the corresponding job schedule. Click the "Edit" button to start editing the job schedule, and click the "Save" button when you completed.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow14.png)

## View Job Schedule Log

Click the "View Log" button in the operation options of a job schedule to view the enabled, disabled, and created jobs of the job schedule for easy tracking of the job schedule.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow15.png)

## Enable/Disable Job Schedule

You can enable/disable the current job schedule by clicking the Enable/Disable button in the "Operation" option in the job schedule list.

![trigger](https://docimages.blob.core.chinacloudapi.cn/images/Console/process/V3workflow16.png)