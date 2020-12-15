# AWS Visual Configuration App Deployment Documentation

### What you need:
- Windows machine with .NET CORE 3.1 or later
- AWS Account and associated Access Keys
- Operating services within your AWS account (services supported as of Iteration 2: EC2, Load Balancer, ECS, and RDS)

### Steps for downloading and launching:

- The executable file can be found in this box link: https://ballstate.box.com/s/vdaj0oxi7jh6ft70nvrcddj2ov8fp7vb
- Download the whole project folder to your computer
- Extract the project files
- Navigate to: AWS-Visual-Configuration-App/bin/release/netcoreapp3.1
- Double click on AWS-Visual-Configuration-App.exe to launch the application
- To close the software, simply close the application window.

### Potential Issues:

**SyncFusion Licensure Warning**
There is currently an erroneous warning that claims the user needs a valid SyncFusion license due to an expiry of the existing licensure.  This is false, and you will simply need to exit out of the error to proceed.  We (the developers) are working with SyncFusion and our client (Accutech) to get this squared away, but communication with SyncFusion is very slow.

**Error Logging**
Currently, there is no error log for users.

**Failed Login:**
- Check for a steady internet connection.
- Check for accurate login credentials.  This could mean your access keys have been refreshed by an AIM administrator on your domain.
- If problems persist, you can log in with only the username. Enter "TestUser" to log in. Note: this will only show the AWS services on the TestUser account.

**Dashboard Issues:**
Service not visible:
- Ensure the service you want to see is currently supported in the application.
- Ensure the service you want to see is running on your AWS account.
- Check for a steady internet connection.
- Refresh services using the refresh button.
- Make sure the service you want to see is selected for visibility under the Settings Menu.  This is accessed using the Settings button on the dashboard. Be sure to click "Refresh" after making changes in Settings.
