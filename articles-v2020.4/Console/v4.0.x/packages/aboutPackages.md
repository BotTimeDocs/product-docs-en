# About Flow Package Management

This page is used to manage the flows uploaded to the console. Flows refer to the automation projects added in Studio. An automation project is called a flow. Users can upload the edited flows to the console. The uploaded flows can be assigned to robots for online running, or generate an online flow library for robots to run locally. Mainly include:

- Upload through Studio
- Manually Upload

## Flow Package Management Permission Description

- View Flow Package: Include the permission to view flow package management menu and flow package management list
- Upload Flow Source File: Include the permission to upload flow
- Delete Flow Package: Include the permission to delete flow package
- Delete Flow Source File: Include the permission to delete flow version file
- Download Flow Source File: Include the permission to download flow

## Flow Package Version

To avoid repeated uploading and the management issues due to flow version update. The system will manage the version of the uploaded flows. If a flow with same package name is uploaded under the same department, the flow is considered as an iterative version of the previous flow and is distinguished by its version number.

Once the flow package version is uploaded, it cannot be modified or overwritten. The user can get all versions of the flow in the flow package. The version contains two states:

- Not used: The version is not selected in the flow execution
- Used: The version is selected in the flow execution