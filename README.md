<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket. This tutorial assumes you have fully completed, installed, set up login credentials, and perform clean up on osTicket in your Virtual Machine environment via following the previous tutorial <a href ="https://github.com/eyenikeyev/osticket-prereqs">"osTicket - Prerequisites and Installation"</a><br />

</br>



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b>

</ul>

</br>

<h2>Post-Install Configuration Objectives</h2>
<ol>
  <li>Familiarity with the UI of osTicket</li>
  <li>Creating and Configuring Roles</li>
  <li>Creation of Tickets</li>
  <li>Creating Agents and Users</li>
  <li>Setting up Service Level Agreements (SLA Plans) in ticketing system</li>
  <li>Configuring Help Topics</li>
</ol>

</br>
<h2>Configuration Steps</h2>


<h3>Configuring Roles, Departments, & Teams</h3>

<p>
  
<ul>


There are two panels when navigating osTicket: Agent Panel and Admin Panel. You will know which panel you're on if the opposite panel is displayed on the top right of the UI next to your user login name. For example the user "eric" is on the Admin Panel
<p>
<img src="https://i.imgur.com/AUpkk7b.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
Configure Roles
<p>
Roles are the permissions granted to Agents per Department that they have access to. Access the Admin Panel, go to Agents tab and click on Roles, then click on Add New Role
<p>
Note: osTicket creates Four Roles - All Access, Expanded Access, Limited Access, and View Only by default.
<img src="https://i.imgur.com/UINgbKj.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
Name the role Supreme Admin, then click on the permissions tab; in this tab you can assign specific permissions to this role. For the Supreme Admin role, check every box under the Tickets, Tasks, and Knowledgebase tabs. Click on Add Role to finish this process
<p>
<img src="https://i.imgur.com/it57abu.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p/>
Configure Departments
<p>

Departments are used to route and resolve tickets based on their importance or instructions. On the Agents tab, click on Departments and click on Add New Department.

Note: osTicket creates two departments (Maintenance and Support) by default
<img src="https://i.imgur.com/lkkCjJL.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Name the Department System Administrators, leave all other options as default, then Create Dept to create department
<img src="https://i.imgur.com/zCcwT0A.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Teams
<p>

The Teams section is used to organize Agents from different departments in osTicket to handle specific issues and supersede Agents and their Departments' parameter rules. Access Admin Panel, in Agents tab, click on Teams and Add New Team.
<p>
Note: osTicket creates a team - Level I Support by default
<p>
<img src="https://i.imgur.com/7ABf8Vr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
Add New Team, name it Level II Support, then click on Create Team
<p>
<img src="https://i.imgur.com/Efmf1ih.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
</ul>
  
</p>

</br>

<h3>Allowing anyone to create Tickets</h3>

<p>
  
<ul>
<p/>
<p>
Access the Admin Panel, go to the Settings tab and click on Users, make sure Registration Required is unchecked. This will allow the user to create tickets anonymously.
<p/>
<p>
<img src="https://i.imgur.com/OEtYw31.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p/>
<p>
</ul>
  
</p>

</br>

<h3>Configure Agents</h3>

<p>
  
<ul>
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
- Go to the agents tab, on the agent section, the user account should be displayed to see that this was done correctly
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
<img src="https://i.imgur.com/KvCRlVK.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
<p/>
Congrats! You've completed everything in this part of the lab
