# Actors
<ul>
<li><b>Users</b><br/>The people using our software</li>
<li><b>Developers</b><br/>The people who made the software</li>
<li><b>AWS APIs</b><br/>APIs which our software will connect to in order to get information</li>
<li><b>Server</b><br/>Whatever is hosting the APIs</li>
<li><b>Admins</b><br/>Can add or remove or modify the permissions of standard users</li>
</ul>

# Use Cases
<ul>
<li>
<b>UC1: Find desired information</b><br/>
Description: This is one of the use cases because the whole purpose of the software is to visualize AWS services and enable the user to find desired information about the services. The user has to be able to do this.<br/>
Actors Involved: User, AWS APIs, Server<br/>
Flow: User opens the application, logs in, and is brought to the main screen. The application connects to multiple AWS APIs, which are hosted on some external server, and gets information. The app displays this information on the main page, allowing the user to look around for the desired information.<br/>
Business Requirement(s): Finding desired information is a part of BR1. In order for B1 to be met, the user must be able to find desired information.<br/>
</li>
<li>
<b>UC2: Be notified of problems</b><br/>
Description: This use case exists and can be exemplified just by opening the software when a problem is occurring.<br/>
Actors Involved: User, AWS API<br/>
Flow: User opens the application, logs in, and is brought to the main screen.  The user immediately becomes aware of a problem, or multiple problems based upon the color of the status text found within the items on the dashboard.  They can then investigate the problem, and address it accordingly.<br/>
Business Requirement(s): This is part of BR1, as being notified of problems should always be considered “desired information,” and it is also a part of BR2 as it shows how the software can “visualize” the AWS service attribute (in this case, a problem) in the same place it is addressed.<br/>
</li>
<li>
<b>UC3: Show and hide information</b><br/>
Description: User should be able to show or hide desired fields, so the user can find the desired information quickly, without having to scroll to locate the information.<br/>
Actors Involved: User<br/>
Flow: User is on the main screen. The user decides they want to see only a few pieces of information, so the user hides all the fields that are not these pieces of information.<br/>
Business Requirement(s): This is part of BR1, because it can help the user find desired information faster. It’s quite possible the user cares about some pieces of information and not others. With this feature, the user can display only the information they care about seeing.<br/>
</li>
<li>
<b>UC4: Toggle between views</b><br/>
Description: User should be able to switch between grid view and diagram view.<br/>
Actors Involved: User<br/>
Flow: User is on the main screen. The user doesn’t want to see the main screen as a diagram view. The user then hits a button, which changes the page’s content layout to a traditional grid view.<br/>
Business Requirement(s): This falls under BR1, because it has the potential to help the user find information faster. Some users might prefer grid view, and can find information faster with grid view. This is also part of BR2, because with either view, information from various AWS services will be visible in one place.<br/>
</li>
</ul>
