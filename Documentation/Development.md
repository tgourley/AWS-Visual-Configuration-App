# AWS Visual Configuration App Development Documentation

### Technology Stack
**Microsoft Visual Studio**

This is the preferred IDE for the project. All instructions in documentation assume the user is using this IDE.  It is a fantastic editor for C#.

**Microsoft .NET CORE framework**

This utility is cross platform and has good ties with AWS.

**Programming Language: C#**

This programming language is compatible with AWS and gives access to frameworks we can use.

**AWS API**

We will utilize AWS API as a “front door” to access important AWS data and functionality.

**AWSSDK.Core**

SDK for .NET that streamlines the use of AWS services. Make sure you have .NET CORE 3.1 or later installed on your machine. (https://dotnet.microsoft.com/download/dotnet-core/3.1/runtime/?utm_source=getdotnetcore&utm_medium=referral)

**Syncfusion Control Library**

Syncfusion has good diagramming tool and has a free claimable licensure.

### Development Environment Replication
##### Required IDE: 
To begin replicating the development environment, first download Microsoft Visual Studio (https://visualstudio.microsoft.com/) 2019 v16.8 or later.
##### Framework: 
When installing Microsoft Visual Studio, install with .NET CORE framework.
##### Clone Repository:
Create a new project by cloning an existing repository. 
GitLab Repository: https://gitlab.com/dark-anvil-labs-cloud-sketch/cloud-sketch.git

### Extensions and Packages: 
Once Visual Studio is installed and the project is open, ensure the that the following Nuget Packages are installed:
- AWSSDK.Core
- AWSSDK.EC2
- AWSSDK.ElasticLoadBalancing
- AWSSDK.S3
- AWSSDK.CloudWatch
- AWSSDK.ECS
- AWSSDK.RDS
- AWSSDK.SecurityToken
- Microsoft.NET.Test.Sdk
- NUnit
- NUnit3TestAdapter
- Syncfusion.SfDiagram.WPF
- Syncfusion.Tools.WPF


### Folder Structure
The project is organized into three main sections. 
1. AWS-API-Configuration-Library contains all API parsing classes. This is organized in order to keep frontend and backend code separate.
2. AWS-Visual-Configuration-App-Tests contains all unit testing for the various aspects of the project.
3. AWS-Visual-Configuration-App contains all front end development such as user interface and backend to front end pipelines. 

### Running the Software (Development)
The software can be ran in Visual Studio by double-clicking "AWS-Visual-Configuration-App," then clicking launching the app by clicking the button of the same name sporting a green triangle.  Once the software is running in Visual Studio, there is a development bar within each window you can use to isolate visual elements, in addition to the normal controls available on the main Visual Studio toolbars.

### Testing
Note: Because running the tests, and hence making many API calls, was incurring a charge, we have implemented mock AWS clients, and the tests now utilize these. In doing so, we are also creating mock AWS items to test the software. 

In order to test this project you need all of the tech stack found ![here](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Design/TechStack.md) with the exception of Slack, which includes administrative access to the Atlassian repository.  You will also need to verify you add the "AWS Toolkit for Visual Studio 2017 and 2019" and "Package Installer" extentions within Visual Studio.

![Get to Test Explorer - Run Tests](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/runtests.JPG?raw=true)
<br/>**Step 1**: Get into test explorer / Run Tests
- After the program has finished building, double-click "AWS-Visual-Configuration-App-Tests" within the solution file, found in Solution explorer.  Once the window has fully opened, right-click the Test container again and select "Run Tests."  This should open the "Test Explorer" window.

![Test Explorer](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/testexplorer.JPG?raw=true)
**Step 2**: Test Explorer
- Test explorer is a fairly complex, but by taking the previous step you should have ran ALL tests for the software in the active branch.  You can access the test structure here, and isolate individual test to run, or select groups.  You can also choose to run only failing tests, or only succeeding tests.  A green checkmark indicates a passing test, and a red X indicates a failing test.

### Determining if the Software is Running Correctly
The software is running correctly if you are greeted by a Login window that allows you to access, view, and, in later iterations, control your AWS services.

### DevMode Option
Because we are working with mock AWS items for testing, we want to verify that these mock items show up in the dashboard properly. The software features a DevMode option, in which the fake items can be viewed. To enable DevMode:

![Login as User](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/logino.jpg?raw=true)
<br/>**Step 1**: Login with Username
- Click "Login with Username". Click on the "o" in the word "Login" three times.

![Blue Box](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/loginbluebox.jpg?raw=true)
<br/>**Step 2**: Blue Box
- After clicking on the "o" three times, a blue box will appear over the "o". Click Login.

![Fake Items](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/fakeawsitems.jpg?raw=true)
<br/>**Step 3**: View Fake AWS Items
- Enabling DevMode successful. Created fake AWS items appear in the dashboard.
