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
3.) Access the Admin Panel
<p>

- click on Agents 
- click on Roles 
- Add New Role
- Name: Supreme Admin
- Go to Permissions section, select all options for Tickets tab, select all options for Tasks tab, check the option for Knowledge Base then Save Changes
<p>
<img src="https://i.imgur.com/pf3q1Xr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
4.) Access the Admin Panel
<p>

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
5.) Access Admin Panel
<p>

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
6.) Access Admin Panel
<p>

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
- primary department: System Administrator
- role: Supreme Admin
- check fall back to primary role on assignments
- leave extended access unselected
<p>

Go to Permissions tab 
- leave everything in there as is
- Go to Teams tab, add Level II Support then Create
- After this go to Agents icon
- Go to Agents tab, the user account should be displayed to see that this was done correctly
<img src="https://i.imgur.com/B01MbYd.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
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
