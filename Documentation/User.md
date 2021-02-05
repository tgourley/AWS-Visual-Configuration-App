# AWS Visual Configuration App User Documentation

### Launch
The program can be launched from the executable found in the root directory you have saved it in.  Double-click the .exe file to run it.  You may have to right-click and select "Run as Administrator" to run it.  Alternatively, it can be ran from visual studio.  See the development environment instructions found [here](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Documentation/Development.md) if that is route you would like to take.

![Login Window - Main](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/loginmain.JPG?raw=true)
### Login Window - Main
The user will have two ways to log in with their AWS account.  Both are presented on the main Login Window, seen above.  The login screen's features are detailed as followed.  Please note that the developer's toolbar and standard window features mentioned occur on every window, and will not be fully explained again later in the documentation, as their functionality does not change.

**Feature 1**: Login with Username
- If you do not have an AWS account, use this method. Log in with the username "TestUser" to see the currently-supported AWS service instances on the TestUser account.  Clicking this button will take you to a further set of window options, detailed below under the heading "Login - Username."

**Feature 2**: Login with Access Keys
- If you have an AWS account, you can use this method. Log in with your AWS username, Access Key, and Secret Key to see the currently-supported AWS service instances on your account.  New users will have to select this method.  Clicking this button will take you to a further set of window options, detailed below under the heading "Login - Access Keys."

**Feature 3**: Login button
- On this screen,  the Login button will be grayed out until the next screen occurs.  This functionality seems redundant at current but will be updated as more complex login features are enabled.  

**Feature 4**: Standard Window Features
- These standard window operators will exist on every window that can be generated within the program.  They allow a user to minimize, maximize, and close the window.  If the window closed is the only window open, the program will also stop.

**Feature 5**: Developer's Toolbar
- This toolbar contains a variety of developer-only features, and will not exist in the production version of the software.  A loose explanation of each button from left to right is: Access Live Visual Tree, Select an Element, Display Layout Adorners, Track a Focused Element, and perform a Hot Reload.  Further explanations of these items can be found on within WPF documentation, found [here](https://docs.microsoft.com/en-us/dotnet/desktop/wpf/introduction-to-wpf?view=netframeworkdesktop-4.8)

![Login Window - Username](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/loginuser.JPG?raw=true)
### Login - User
After clicking the "Login with Username" button, these options will appear.

**Feature 1**: Username Entry
- Enter a valid AWS username here.  Failure to enter a valid username entered will result in an error prompt, and you may try again or proceed to exit the program.

**Feature 2**: Home Button
- Clicking this will return you to the previous menu, detailed above under "Login Window - Main."

**Feature 3**: Login Button
- On this menu, this button will be available.  Clicking it with a valid username will allow you further into the program by accessing your relative AWS account.

![Login Window - Access Keys](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/loginaccess.JPG?raw=true)
### Login - Access Keys
After clicking the "Login with Access Keys" button, these options will appear.

**Feature 1**: Home Button
- Clicking this will return you to the previous menu, detailed above under "Login Window - Main."

**Feature 2**: Username Entry
- Enter a valid AWS username here.  Failure to enter a valid username will result in an error prompt, and you may try again or proceed to exit the program.

**Feature 3**: Access Key Entry
- Enter a valid AWS access key.  Failure to enter a valid access key will result in an error prompt, and you may try again or proceed to exit the program.

**Feature 4**: Secret Key Entry
- Enter a valid AWS secret key.  Failure to enter a valid secret key will result in an error prompt, and you may try again or proceed to exit the program.

**Feature 5**: Save Login
- Checking this will allow your AWS information to be saved locally, and allow for quicker login with the "Username" option on the primary Login menu next time you access the software.

**Feature 6**: Login Button
- On this menu, this button will be available.  Clicking it with a valid username, access key, and secret key will allow you further into the program by accessing your relative AWS account.

![Dashboard](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/mainwindowmain.JPG?raw=true)
### Dashboard
The dashboard above will be presented when you log in successfully.  The AWS services that appear are specific to your/your employer's account, and also may vary based upon the settings feature, which is detailed below. NOTE: the first time you use this application, you may notice that the dashboard is empty. If this is the case, click on Settings, check all the AWS service boxes, close Settings, then hit Refresh.

**Feature 1**: Drop-Down View
- This view shows basic information such as instance ID's and whether or not the service is running in a static format for your various AWS services.  You can expand or collapse items to see nested services.  Clicking a service here will focus it both in this view, and in the Visualization view, which is detailed below.

**Feature 2**: Load Balancer Representation / Secondary Service
- The icon indicated in the picture represents a load balancer.  In future iterations, it may be used as a general icon for a service type that touches multiple other services, also known as a secondary service.

**Feature 3**: EC2 Representation / Primary Service / Currently Focused Indication
- The icon indicated in the picture represents an EC2 instance.  In future iterations, it may be used as a general icon for a primary service type.  This particular EC2 also shows what an object looks like when it is "focused."

**Feature 4**: Zoom-In / Zoom-Out
- These buttons can be clicked to zoom in and out on the visualizatin menu.  They are detailed a bit further below under the "Zoom-In - Zoom-Out" heading.

**Feature 5**: Logout Button
- This button returns a user to the primary login screen.

**Feature 6**: Settings Button
- This button takes a user to the settings menu, detailed below under the heading "Settings Menu."

**Feature 7**: Refresh Button
- This button allows a user to refresh their active connection to AWS.  If a change is made using the Amazon Dashboard, you can click this to see relevant changes reflected.  Additionally, after making changes in the Settings Menu, you can click this to see the changes.

**Feature 8**: Visualization View
- This pane visualizes your AWS services and displays similar, relevant information for each service.

![Zoom-In - Zoom-Out](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/dragonzoom.JPG?raw=true)
### Zoom-In - Zoom-Out
When zoomed-in sufficiently, drabbable sliders appear to allow finer control of the pane.

![Settings Menu](https://github.com/welawrence543/AWS-Visual-Configuration-App/blob/master/Auxiliary%20Files/servicesettings.JPG?raw=true)
### Settings Menu
This menu allows you to control which services are show on the dashboard.

**Feature 1**: Select Service Category
- Right now there is only one nested category, but this will change with further iterations.  Eventually, this will be used to quickly find which services you want to adjust visibility of.

**Feature 2**: Select Service Checkboxes
- Select or deselect checkboxes to add or remove services to your dashboard display.

**Feature 3**: Exit Menu
- Click the standard "Exit" window operator to exit the window and save changes.  You will have either click "Refresh" or logout and log back in to see the reflected changes.

### The following are services supported by iteration 2 release.
- EC2
- Load Balancer
- RDS
- ECS
- S3
