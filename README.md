<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLAs
- Configure Help Topics

<h2>Configuration Steps</h2>
1.) Go to https://portal.azure.com/, connect to Remote Desktop Connection with the virtual machines' Public IP Address, enter the username and password
</p>
2.) Browse to your help desk login page: http://localhost/osTicket/scp/login.php, this is only accessible while in the virtual machine
</p>
<img src="https://i.imgur.com/d2eYZol.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
3.) Configure Roles
<p>

- access the admin panel
- click on Agents 
- click on Roles 
- Add New Role
- Name: Supreme Admin
- Go to Permissions section, select all options for Tickets tab, select all options for Tasks tab, check the option for Knowledge Base then Save Changes
<p>
<img src="https://i.imgur.com/pf3q1Xr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
4.) Configure Departments
<p>

- access the admin panel
- click on Agents
- click on departments
- click on Add a New Department
- Name: System Administrators
- Ticket Assignment: All
- Leave the rest of the options as default
- Create Department
<img src="https://i.imgur.com/PjDwRbZ.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
5.) Configure Teams
<p>

- access admin panel
- click on Agents tab
- click on Teams tab
- Add New Team
- Name: Level II Support
- leave other options as default
- click on Members
- add yourself as an agent
- Create Team
<img src="https://i.imgur.com/LM5R2nT.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
6.) Configure Agents
<p>

- access admin panel
- click on Agents tab
- Add New Agent
- Name: Jane Doe
- email: janedoe@osticket.com
- username: jane.doe
- select Set Password
- uncheck the send the agent a password email reset
- password: Password1
- uncheck require password change at next login
- Set, then leave the rest
<p>

Go to Access tab
<p>

- primary department: System Administrator
- role: Supreme Admin
- check fall back to primary role on assignments
- leave extended access unselected
<p>

Go to Permissions tab 
<p>

- leave everything in there as is
- Go to Teams tab, add Level II Support then Create
- Go to Agents tab, on the agent section, the user account should be displayed to see that this was done correctly
<img src="https://i.imgur.com/B01MbYd.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Access Admin Panel
<p>

- click on Agents tab
- Add new agent
- Name: John Doe
- email: johndoe@osticket.com
- username: john.doe
- select Set Password
- uncheck the send the agent a password email reset
- password: Password1
- uncheck require password change at next login
- Set, then leave the rest
</p>
<p>
Go to Access tab
<p>

- primary department: Support
- Select Role: View Only
- Extended Access: Support
- then Create
- After this go to the Agents icon
- Go to the agents tab, the user account should be displayed to see that this was done correctly
</p>
<p>
<img src="https://i.imgur.com/AThQTw4.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
7.) Configure Users
<p>

- Go to Agent Panel
- Users tab
- Add User
- email: Karen@osticket.com
- Full Name: Karen Smith
- Add User
<p>

Go to Agent Panel
- Users tab
- Add User
- email: Ken@osticket.com
- Full Name: Ken Smith
- Add User
</p>
<p>
8.) Configure SLAs
<p>

- Access Admin Panel
- Manage tab
- select SLA
- Add New SLA plan
- Name: SEV-A
- Grace period: 1 hour
- Schedule: 24/7
- then Add Plan
<p>
</p>
Add New SLA plan
<p>

- Name: SEV-B
- Grace period: 4 hours
- Schedule: 24/7
<p>
</p>
Add New SLA plan
<p>

- Name: SEV-C
- Grace period: 8
- Schedue: Monday-Friday 8:00 AM - 5 PM
<p>
Go to the Manage tab, on the SLA section, the SLAs should be displayed to see that this was done correctly
<p>
<img src="https://i.imgur.com/nn3SSIP.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
9.) Configure Help Topics
<p>

- Access Admin Panel
- Manage tab
- Add New Help Topic
- Topic: Business Critical Outage
- Parent Topic: Top Level Topic, leave other options as default
- Add topic
<p>
</p>
Add New Help Topic
<p>

- Topic: Personal Computer Issues
- leave other options as default
- Add topic
<p>
</p>
Add New Help Topic
<p>

- Topic: Equipment Reset
- leave other options as default
- Add topic
<p>
<p/>
Add New Help Topic
<p>

- Password Reset
- leave other options as default
- Add topic
<p>
Go to the Manage tab, on the Help Topics section, the Help Topics should be displayed to see that this was done correctly
<p>
<p/>
<img src="https://i.imgur.com/EIHrb7X.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
