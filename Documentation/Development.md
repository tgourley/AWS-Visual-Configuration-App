# AWS Visual Configuration App Development Documentation

### Technology Stack
**Microsoft Visual Studio**

This is the preferred programming environment for the project. It is a fantastic editor for C#.

**Microsoft .NET CORE framework**

This utility is cross platform and has good ties with AWS.

**Programming Language: C#**

This programming language is compatible with AWS and gives access to frameworks we can use.

**AWS API**

We will utilize AWS API as a “front door” to access important AWS data and functionality.

**AWSSDK.Core**

SDK for .NET that streamlines the use of AWS services. 

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

### Testing
All testing can be found in the AWS-Visual-Configuration-App-Tests folder. Running unit tests ensures functioning code. In the event of an error or failed unit test, use the unit tests to find the dysfunctional code. 

To run all tests, click Test -> Run All Tests. 
In Test Explorer, red X's flag failed tests and green checkmarks show passed tests.

As far as the application itself, launch the program within Visual Studio. Log in with your own AWS credentials. Once logged in, you will find an interface displaying various details of services that currently supported. 
Currently supported services include: 
- EC2
- Load Balancer
