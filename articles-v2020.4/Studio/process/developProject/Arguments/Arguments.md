# Parameter

**Parameters** are used to pass data from a project to another project. In a global sense, they are similar to variables in that they dynamically store data and pass it around. Variables pass data between activities, while parameters pass data between automation flows. As a result, they enable you to reuse the automation flows time and time again.

The ENCOO RPA studio supports a large number of parameter types that are consistent with variable types. Thus, you can create parameters of String, Boolean, Object, Array, or DataTable type, as well as browse .Net type, which is the same as variables.

In addition, parameters are passed in specific directions (input, output, input/output, property) that tell the application where the information stored in them should be passed to.

## Create Parameter

> **Note:**
> 
> The parameter name should be prefixed on the hump to indicate the direction in which the parameter is passed.
> 
> For example, in\_DefaultTimeout, in\_FileName, out\_TextResult, io\_RetryNumber.

To create a new parameter:

1. In the "Editing Area", click "Parameters". Then a list of parameters will be displayed.
   
    ![Create Parameter](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Argument/argumentPanel-createArgument.png)

2. Click on the "Create Parameter" line. A new parameter with the default field value will be displayed.

 > **Note:**
 > 
 > By default, all parameters are of type String in the input direction.

## Delete Parameter

1. In the list of parameters, select a parameter and right-click on it. Then click on the "Delete" option in the context menu.
   
    ![Delete Parameter](https://docimages.blob.core.chinacloudapi.cn/images/Studio/Argument/deleteArgument.png)

2. In the parameter list, select a parameter and press Delete.

> **Note:**
> 
> To undo this operation, press Ctrl + Z.