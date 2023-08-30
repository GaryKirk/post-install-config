<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
The aim of this lab is to correctly configure osTicket, an open-source ticketing system. I completed this lab to gain a better understanding of the skills involved in working as an System Administrator and Desktop Support Technician in an IT Department.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

A - To gain experience configuring the following areas of osTicket:
<ul>- Roles</ul>
<ul>- Departments</ul>
<ul>- Teams</ul>
<ul>- Workers</ul>
<ul>- Users</ul>
<ul>- Service Level Agreements</ul>
<ul>- Help Topics</ul>
B - To gain an understanding of how to read software documentation and put what is learned in to practice.

<h2>osTicket Configuration Setup</h2>
<p>1. In Remote Desktop, connect to the Windows VM using the public IP address found in Microsfot Azure. Use your VM login details to connect. After connection to the VM, open a browser window and go to <a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a>. Use your osTicket Admin credentials to login to osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/e8ae316c-1a62-4996-96b4-51c79f2ca50e" alt="Login to osTicket as Admin" width="500" length="500"/><br /><br />

<p>2. In the top-right, click to go to the 'Admin Panel'. From here click Agents --> Roles --> Add New Role. Name the new role "Supreme Admin". Under the 'Permissions' tab, click to allow all permisisons in 'Tickets'. Click to save the changes. The Supreme Admin role now has access to all permisisons in osTicket. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">Roles Documentation</a> to find out more about how Roles work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/748a8368-8692-4e85-a9ce-cdb038e4d9a1" alt="Roles" width="500" length="500"/><br /><br />

<p>3. To setup a new department, click Agents --> Departments --> Add New Department. Name the new department "System Administrators". Leave all other settings as default. Click to save the changes. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">Departments Documentation</a> to find out more about how Departments work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/6e129827-b365-4923-a4e3-fcf524a9f846" alt="Departments" width="500" length="500"/><br /><br />

<p>4. Next, to setup a new Team, click Agents --> Teams --> Add New Team. Name the new team "Level II Support". On the members tab, use the drop down menu to add yourself to the team. Click to save the changes. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Team Documentation</a> to find out more about how Teams work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/01bb2179-d32b-4db1-92d0-0b63b37f15e7" alt="Teams" width="500" length="500"/><br /><br />

<p>5. Next, to setup a new Team, click Agents --> Teams --> Add New Team. Name the new team "Level II Support". On the members tab, use the drop down menu to add yourself to the team. Click to save the changes. Read the <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">Teams Documentation</a> to find out more about how Teams work in osTicket.</p>
<img src="https://github.com/GaryKirk/post-install-config/assets/137613637/01bb2179-d32b-4db1-92d0-0b63b37f15e7" alt="Teams" width="500" length="500"/><br /><br />

