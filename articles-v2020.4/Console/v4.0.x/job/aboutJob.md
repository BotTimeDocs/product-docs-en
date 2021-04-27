# About Job Records

**This feature is only available in Enterprise Edition**

The Job Records page is mainly used to record and display the execution conditions of all flow jobs, and to manage the job execution log in a comprehensive manner. In this page, you can view the job execution conditions and results, and also view the job log.

> **Description:**
> 
> - This page displays all flow jobs created by job schedule or manual execution for all flow deployments;
> - The "Job List" in the "Flow Deployment" module only displays the job records of that flow deployment.
> - The "Job List" in the "Scheduling Queue" module only displays the job created and scheduled in the scheduling queue.

In this page, you can view the job execution conditions and results. For the job that has been executed, you can also view the job log.

## Execution Queue State Description

- **Waiting**: The job is queuing, and the robot is **busy** or has **no response**
- **Running**: The robot is executing the job
- **Aborted**: The job is forcibly aborted by the user
- **Failed**: The job is executed, and the return result is failed
- **Successful**: The job is executed, and the return result is successful

## Execution Queue Permission Description

- **View Execution Queue**: Include the permission to view the execution queue menu, and the permission to view and search the execution queue
- **Manage Execution Queue**: Include the permission to abort, execute with priority, re-execute the execution queue.