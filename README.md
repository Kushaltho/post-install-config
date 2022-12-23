<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Before Starting, Finish:</h2>

[osTicket: Prerequisites and Installation](https://github.com/Kushaltho/osticket-prereqs)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles,Teams, Departments,
- Add Agents/workers and Users/Customer
- Configure Agents and Users with appropriate Roles,Teams and Deparments
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h3> Step 1</h3>


<p>
<img src="https://i.imgur.com/fHQwy5U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>   
<img src="https://i.imgur.com/pmsDRxP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>

  If you had stopped and taken a break after the Installation then, 
  
  Start the VM , remote into the VM, go to http://localhost/osTicket/scp/login.php in the VM and login using the credentials you made.
 
  And a similar page should open up.
</p>
<br />



<h3> Step 1</h3>
<p>
<img src="https://i.imgur.com/Bob96DS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Quick Difference between an admin and agent is that an admin(job title usally system admin) sets up the osticket enironment/settings like SLAs while the agent(help desk) will work through the tickets. You will have a much clearer understanding after completing the whole walkthrough.
    

    Admin Panel -> Agents -> Roles -> Add New Role

    Create Admin

    We will just allow it every permission 
 
</p>
<br />




<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Deparments are used to divide and class so that when errors/tickets come through it can be directed towars the right deparemnt such as when there is a subnetting problem we would send it to the networking department.
    
    Configure Departments

    Admin Panel -> Agents -> Departments

    Create System Administrators
    

</p>
<br />


<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Teams
Admin Panel -> Agents -> Teams
Level I Support
Level II Support

</p>
<br />


<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Allow anyone to create tickets
Admin Panel -> Settings -> User Settings
Registration Required: Require registration and login to create tickets 

</p>
<br />


<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane
John

</p>
<br />


<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

</p>
<br />


<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (1 hour, 24/7)
Sev-B (4 hours, 24/7)
Sev-C (8 hours, business hours)

</p>
<br />

<h3> Step 1</h3>
<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configure Help Topics
  
Admin Panel -> Manage -> Help Topics
  
Business Critical Outage
  
Personal Computer Issues
Equipment Request
Password Reset


</p>
<br />
