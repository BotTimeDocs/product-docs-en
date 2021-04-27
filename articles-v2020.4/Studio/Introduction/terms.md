# Product Glossary

Before using ENCOO RPA Studio, you must understand the following concepts.

## Flow Project

A flow project is a collection of all the flow files used to manage all the flows associated with a single automation job.

For example, if you need to create an automation flow that handles customer orders on a regular basis, you can create a flow project in which all subflow files, dependencies, and other information related to this job will appear. Flow project is the basic unit that you develop, publish, and deploy to robots for running. Typically, a new flow project shall be created for each separate job.

## Flow File

A flow file is a source file that describes the flow logic, usually in the format of .xaml.

Each flow project has only one main flow file, Main.xaml by default, which is the starting point for robot execution. Main.xaml is the default file for each flow project and cannot be deleted. Also, you can add multiple subflow files to your project for writing subflows, and the main flow and subflow are callable from each other.

It is suggested that relatively independent parts of the flow can be placed in a subflow file, which has two advantages:

1. Convenient to be called repeatedly by multiple flows;
2. Simplify the main flow, and facilitate the maintenance and updating in the future.

## Activity

An activity is the basic unit that makes up a flow, describing an action in the flow, such as opening a website, clicking a button, entering text in an input box, etc.

The process of creating a flow is a matter of dragging the correct activities into the flow editing area. So activity is the most important content in the process of learning Studio, being familiar with the use of various activities, you can soon become a master of automation flow editing.

## Variable

Variables are used to store temporary data for the flow execution process, with the same meaning as variables in any programming language.

The flow execution engine of ENCOO RPA Studio is strengthened, so variables will have different types, such as integer type, string type, etc. The main purpose of using variables is to pass data in the flow, for example, the text information from a web page can be stored in a variable, processed, and then used by another activity.

## Parameter

Arguments are used to accept data from the flow caller, the same as the arguments of functions in any programming language.

Both the main flow and the subflow can have arguments, and the corresponding values can be passed in when calling this flow, which can achieve the purpose of passing in different data each time the flow is called. If an argument is not required, you can set a default value for it.