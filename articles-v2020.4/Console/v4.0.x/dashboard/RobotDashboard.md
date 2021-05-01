# Robot Monitoring

**This feature is only available in Enterprise Edition**

The Robot Monitoring page allows you to view the status of your robot by today, the last 7 days, the last 30 days, or a custom time period, as shown in the figure below.

![Robot Monitoring](https://docimages.blob.core.chinacloudapi.cn/images/Console/Dashboard/EnV4Dashboard2.png)

| No.| Parameter| Description
|----------|----------|----------
| 1| Available Robot Job Execution Count| Count the number of flows executed by all robots under the current department in the current time range.
| 2| Total Available Robot Busy Time| Count the total amount of buy time of all robots under the current department in the current time range (the accumulated busy time of all robots).
| 3| Average Available Robot Busy Ratio| Count the average busy ratio of all robots under the current department in the current time range (the total amount of busy time of all robots / the total amount of presence time of all robots in the current time range).
| 4| TOP10 Available Robot Failure Rate| Count the distribution of the total number of flows that failed. <br> Percentage of failures of each robot = number of flows that failed for the current robot / total number of flows that failed during the period. For example, if 100 of 1000 runinstances failed on robot A, the failure ratio would be calculated as 10%.
| 5| Available Robot Status Distribution| Count the status distribution of all robots under the current department in the current time range. Robot status includes licensed, unlicensed, interrupted, busy, idle.
| 6| TOP10 Total Available Robot Busy Time| Display how busy all robots under the current department are (the number of flows executed) as well as the specific flow package.

