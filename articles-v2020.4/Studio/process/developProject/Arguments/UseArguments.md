# Use Arguments

Arguments allow you to pass data from a flow file to another. They are mainly used in the Call Flow activity, which could be found in the Activities panel under Flow Control.

## Example of Usage

How do we use arguments in the Call Flow activity? We are going to create two sequences, and pass data between these two sequence flow files, finally write the data to log. The details are as follows:

1. Open Studio, create a project, and add a subflow file named Argument1 to the project.

2. Open the arguments list, create an Out argument (outData) with the type of String.

3. Add an Assign activity to the Flowchart from the Activities panel.

4. In the Properties panel of "Assign", enter the following content:
   
   * Variable name: outData
   * Value: "Excuse me, what is your name?"

5. At this point, the subflow file is as shown below: 

    ![Subflow File](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/outdata20210430.png)

6. Open the Main.xaml file, open the variable list, and create an argument (result) with the type of String

7. Drag in a Call Flow activity from the Activities panel

8. Double click to open the activity, click "..." to browse folders, select the previously created Argument1.xaml file

9.  Click "Set Arguments" to display the Edit Arguments window, where you add the arguments from the Argument1.xaml file
   
   * Name: outData
   * Direction: Output
   * Type: String
   * Value: result

11. Drag in "Write to Log" activity and connect to "Assign" activity

12. In the Properties panel of "Write to Log", enter the following content:
    
    * Log content: "result+" My name is Xiaojiang. ""

13. At this point, the main flow file is as shown below:
    
    ![Main Flow File](https://docimages.blob.core.chinacloudapi.cn/images/EnglishDocumentImage/themainflow20210430.png)

Finally run the flow and the Output panel will display the relevant information.