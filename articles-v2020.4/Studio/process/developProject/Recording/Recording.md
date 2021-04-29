# Smart Recording

**Smart recording** is an important part of the ENCOO RPA studio, that can help you save a lot of time when automating your business flows. This feature enables you to easily capture a user’s actions on the screen and translates them into sequences.

Using the recording feature, after recording the automation flow projects, you can modify these projects and adjust the corresponding parameters so that you can easily recall them in other flows.

## Recording Description

When a yellow rectangular box appears in the interface, it means recording has started. At this point, you can click on the target element, as the rectangle represents the identified element. It also means you can click on it to get data or otherwise interact with it. As shown in the image below, in this way, you can be sure the correct buttons, texts, or menus are selected.

![Recording](https://docimages.blob.core.chinacloudapi.cn/images/Studio/recording/recording.png)

Interactions with UI elements during recording yield informative screenshots. Regardless of the type of recording selected, some actions are recordable and some are not.

- **Recordable Actions**
  
  - Left-click on buttons, check boxes, drop-down lists, and other GUI elements
  - Text typing

- **Non-Recordable Actions**
  
  - Keyboard shortcuts

> **Note:**
> 
> If you make changes to your display settings without restarting the computer, elements are not going to be properly identified.

## Recorder

There are two main types of recording in the ENCOO RPA studio, that is, website recording and desktop recording.

All recording types use the same recorder, which is designed to record actions in web applications and desktop applications. It allows you to record actions in a variety of operating environments.

The recorder enables you to:

- Automatically record multiple actions performed on the screen

- Manually record single actions, such as:
  
  - Clicking or double-clicking an interface element
  - Entering text into the text box
  - Looking for elements or waiting for them to disappear

Keyboard shortcuts that you can use while recording:

- F2 - pauses for 5 seconds.

- Esc - exits the recording.

- Ctrl+mouse dragging frame - image recognition.

- F4 - switches the recording technology.
  
  | Recording Technology| Description
  |----------|----------
  | Automatic| It includes</br> - JAB for recording desktop elements (JAVA application), SAP (SAP system application) recording technology</br> - IE, Chrome, Firefox, Edge, 360 browser recording technology for recording Web elements, where the Web elements recording technology makes it possible to automatically match the corresponding recording technology according to the browser type.
  | IA| For special applications, IA recording technology is used.
  | UIA3(UIA)| It is used for non-special applications. </br> The difference between UIA3 and UIA lies in the different levels of support for different technologies. </br> - UIA3 has a higher level of support for WPF and Windows Store Apps; </br> - UIA has a higher level of support for C# and WinForms.



### Recorder Interface Actions

- **Recorder Interface**

![Recorder](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/smartrecorder20210429.png)

| Options| Description
|----------|----------
| Smart Recording| Click on it to start recording a website or desktop application.
| Save \& Exit| Save the recorded automation flow to the ENCOO RPA studio and exit the recorder.
| Clear| Remove the automation flow recorded in the recorder.
| Click| It is divided into three types, that is, click, double click, and select. </br> Click/Double-click: Manually perform a click/double-click action on an interface element. </br> Select: Select an interface element.
| Text| It is divided into two types, that is, get text and input text. </br> Get text: Used to get the content of the text. </br> Input text: When there is no content in the text box, you can add text content directly to the text box.
| Event| It is divided into two types, that is, wait for elements to appear and wait for elements to disappear. It is mainly used for judgment. </br> Wait for elements to appear: Wait for interface elements to appear. </br> Wait for elements to disappear: Wait for interface elements to disappear.

- **Recorder Preview Interface**

When the recorder has recorded some automated actions, a preview interface shall be generated. In this interface, you can change and delete the recorded actions to refine your automation flow.

![Preview Interface](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/recorderpreviewinterface20210429.png)