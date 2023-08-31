<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
The aim of this lab is to correctly configure osTicket, an open-source ticketing system. I completed this lab to gain a better understanding of the skills involved in working as an System Administrator and Desktop Support Technician in an IT Department.<br />

<h2>Environments and Technologies Used</h2>

<ul>
  <li>Microsoft Azure (Virtual Machines/Compute))</li>
  <li>Remote Desktop)</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

A - To gain experience configuring the following areas of osTicket:
<ul>
  <li>Roles</li>
  <li>Departments</li>
  <li>Teams</li>
  <li>Workers</li>
  <li>Users</li>
  <li>Service Level Agreements</li>
  <li>Help Topics</li>
</ul>

B - To gain an understanding of how to read software documentation and put what is learned in to practice.

<h2>osTicket Configuration Setup</h2>
<p>1. In Remote Desktop, connect to the Windows VM using the public IP address found in Microsfot Azure. Use your VM login details to connect. After connection to the VM, open a browser window and go to <a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a>. Use your osTicket Admin credentials to login to osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/e8ae316c-1a62-4996-96b4-51c79f2ca50e" alt="Login to osTicket as Admin" width="500" length="500"/><br /><br />

<p>2. In the top-right, click to go to the 'Admin Panel'. From here click Agents --> Roles --> Add New Role. Name the new role "Supreme Admin". Under the 'Permissions' tab, click to allow all permisisons in 'Tickets'. Click to save the changes. The Supreme Admin role now has access to all permisisons in osTicket. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Roles Documentation</a> to find out more about how Roles work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/748a8368-8692-4e85-a9ce-cdb038e4d9a1" alt="Roles" width="500" length="500"/><br /><br />

<p>3. To setup a new department, click Agents --> Departments --> Add New Department. Name the new department "System Administrators". Leave all other settings as default. Click to save the changes. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Departments Documentation</a> to find out more about how Departments work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/6e129827-b365-4923-a4e3-fcf524a9f846" alt="Departments" width="500" length="500"/><br /><br />

<p>4. Next, to setup a new Team, click Agents --> Teams --> Add New Team. Name the new team "Level II Support". On the members tab, use the drop down menu to add yourself to the team. Click to save the changes. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Teams Documentation</a> to find out more about how Teams work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/01bb2179-d32b-4db1-92d0-0b63b37f15e7" alt="Teams" width="500" length="500"/><br /><br />

<p>5. In order to allow all users to add tickets to the system, a setting can be toggled on. To do this, go to Settings --> User Settings. Under 'Authentifiction Settings', make sure that 'Require registration and login to create tickets' is unchecked. This will allow anyone to add tickets. If you would prefer users to be registered before adding tickets, you can check the box.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/4bc29089-08a7-4c43-8a03-af1e97427368" alt="Settings for Adding Tickets" width="500" length="500"/><br /><br />

<p>6. To add agents, who will work on incoming tickets, click Agent --> Add New Agent. On the following screen, add the agent's name and email address. Also, setup a username and password for the agent. Under the corresponding tabs, setup the agents department access, permissions, and team. Click to create the agent. Complete the process again to add more agents. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">Agents Documentation</a> to find out more about how Agents work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/78035b91-c86b-4c63-82ff-4d6f8ee7f1e5" alt="Agents" width="500" length="500"/><br /><br />

<p>7. In order to setup new users, who can add tickets to the system, click Agents Panel --> Users --> Add User. On the following screen, add the user's name and email address. Click to save the changes. Complete the process again to add more users. Read the <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">Users Documentation</a> to find out more about how Users work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/c084a89b-91e0-4ad2-9c3a-e8e2c32e97e8" alt="Users" width="500" length="500"/><br /><br />

<p>8. To configure Service Level Agreement Plans, which set out in detail how certain issues and users should be handled, click Admin Panel --> Manage --> SLA --> Add New SLA Plan. Following this, use the Name, Grace Period, and Schedule information below to setup three different SLAs. After each one is complete, click to save the changes.</p>
<ul>
  <li>Sev-A (1 hour, 24/7)</li>
  <li>Sev-B (4 hours, 24/7)</li>
  <li>Sev-C (8 hours, business hours)</li>
</ul>

<p>Read the <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">SLA Documentation</a> to find out more about how SLAs work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/3c4348e1-bfd3-458d-ba5b-f2f31fa60c57" alt="SLAs" width="500" length="500"/><br /><br />

<p>9. Help Topics are used by users to provide information about their issue. To setup some common Help Topics, click Admin Panel --> Manage --> Help Topics --> Add New Help Topic. Use the details below to setup four different Help Topics. After each one is complete, click to save the changes.</p>
<ul>
  <li>Business Critical Outage</li>
  <li>Personal Computer Issues</li>
  <li>Equipment Request</li>
  <li>Password Reset</li>
</ul>

<p>Read the <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html">Help Topics Documentation</a> to find out more about how Help Topics work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/24e5fb2c-1516-40b2-bb2e-0b27c5ef8c8c" alt="Help Topics" width="500" length="500"/><br /><br />

The core settings of osTicket are now configured correctly. The system is ready to receive, manage, and complete help desk tickets.

