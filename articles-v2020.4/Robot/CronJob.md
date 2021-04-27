# Cron Job

Supports creating a cron job and automatically executing the related flow at the specified time.

## New Cron Job

Click **New Cron Job** to open the Cron Job window, as shown in the following figure:

- Job Name: Enter a cron job name.

- Flow: Select Local flow library or Console flow library, and then select the flow and version to be executed in the cron job.
  
  > **Description:**
  > 
  > You can click Execution Config to open the Execution Config dialog box and configure parameters for the flow execution. See [Executing Local Flows](Robot/../localworkflow.md).

- Mode: select an execution mode. The optional modes are Once, By Day, By Week, By Month, and By Expression.
  
  | Parameter| Description                                                     |
  | -------- | ------------------------------------------------------------ |
  | Once| The cron job is executed only once. The default is the current date and time.
  | By day| The cron job is executed every N days. The default interval is one day. The default execution time is the current time.
  | By week| The cron job is executed on the Xth day of the week every N weeks. The default interval is one week. The default execution time is the current time.
  | By month| The cron job is executed on the Xth day of the month every N months. The default is the first day of every month. If X is greater than the maximum number of days in a month, the default is the last day of this month. <br> The cron job is executed on the Yth day of the Mth week every N months. The default is the first Sunday of every month. The default execution time is the current time.
  | By expression| Configure the cron job by [Cron](https://baike.baidu.com/item/cron/10952601?fr=aladdin) expression. <br> Click [Online Generator](https://console.encoo.com/lib/cron/index.html) to generate a Cron expression online and then copy the expression to the Cron expression text box.


- Time Range:
  
  - Start time: the time when the job is activated. The default start time is the current time if you do not fill this field.
    
    > **Description:**
    > 
    > A prompt window pops up in the bottom right corner of the desktop and starts counting down at 30 seconds before the job is activated.

- End time: the time when the job expires. If you do not enter this field, the job never expires.

![Cron job setting](https://docimages.blob.core.chinacloudapi.cn/images/Robot/cronjob20201201.png)

## Cron job list

Each job row in the cron job list contains:

- Job: The name of the cron job
- Flow Library: The flow library to which the flow in the cron job belongs
- Flow: the name of the flow in the current cron job
- Mode: the execution mode of the current cron job
- Operation: Click **Edit** to modify the current cron job. Click **Delete** to remove the current cron job.

![Cron job list](https://docimages.blob.core.chinacloudapi.cn/images/Robot/Robot-CronJob-1.png)