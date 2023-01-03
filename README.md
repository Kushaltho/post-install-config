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
- Configure Agents and Users with appropriate Roles,Teams and Departments
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h3> Step 1 Open VM and Login</h3>


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



<h3> Step 2 Configure Roles</h3>
<p>
<img src="https://i.imgur.com/Bob96DS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Quick Difference between an admin and agent is that an admin(job title usually system admin) sets up the osticket environment/settings like SLAs while the agent(help desk) will work through the tickets. You will have a much clearer understanding after completing the whole walkthrough.
    

    Admin Panel -> Agents -> Roles -> Add New Role

    Create Admin

    We will just allow it every permission 
 
</p>
<br />




<h3> Step 3 Configure Departments</h3>
<p>
<img src="https://i.imgur.com/UldqTwt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Departments are used to divide and class so that when errors/tickets come through it can be directed towards the right department such as when there is a subnetting problem we would send it to the networking department.

    Admin Panel -> Agents -> Departments

    Create department "System Administrators"
    
    Leave the default settings

</p>
<br />


<h3> Step 4 Configure Teams</h3>
<p>
<img src="https://i.imgur.com/65gUw4E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/ivI7jVD.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In osTicket, "teams" are groups of users who work together to manage and respond to customer inquiries, issues, and requests. An administrator creates and configures teams to fit the specific needs and workflow of an organization.
  
    Admin Panel -> Agents -> Teams
  
    Create "Level II Support"
  
    Differences between the teams can be up to the organization. For example, Level II Support might have people with more expertise than I.

</p>
<br />


<h3> Step 5 Allow anyone to create tickets</h3>
<p>
<img src="https://i.imgur.com/dmnhEM7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Allow anyone to create tickets even if they are not a user in the System. However, we will require them to register and login.
  
    Admin Panel -> Settings -> User Settings
  
    Registration Required: Require registration and login to create tickets 

</p>
<br />


<h3> Step 6 Configure Agents </h3>
<p>
<img src="https://i.imgur.com/id6Saks.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/IssElwr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/dGsKyNX.png" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/ff64E4O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Configure Agents (workers), who are usually able to view, update, and manage customer tickets within the system.
    
When creating a password for the agents have the settings shown above. However,it is just for the walk-through as you might want to turn that on for security. .

Assign them the appropriate roles,permissions, departments, and teams.
  
Names and emails are up to you.
  
    Admin Panel -> Agents -> Add New
    
    Create "Kevin" and "Evelyn"
  
    
    
    

</p>
<br />


<h3> Step 7 Configure Users </h3>
<p>
<img src="https://i.imgur.com/GAp9Ya7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Users are the ticket owners of the tickets in the help desk. When a ticket is created in the help desk, the user is associated with their email address.
  
Names and emails are up to you.

    Agent Panel -> Users -> Add New

    Create "Andrew" and "Zuquan"

</p>
<br />


<h3> Step 8 Configure SLAs</h3>
<img src="https://i.imgur.com/eW8zOjG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZakDWXP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/gEgMP3C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
SLA might outline the response times and resolution times that the service provider promises to deliver for (tickets)customer inquiries or issues. 

But as a worker for the service provider it shows the severity of the issue/ticket.

    Admin Panel -> Manage -> SLA

    Sev-A (1 hour, 24/7)

    Sev-B (4 hours, 24/7)

    Sev-C (8 hours, business hours)

</p>
<br />

<h3> Step 9 Configure Help Topics </h3>
<p>
<img src="https://i.imgur.com/rdcsle7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Help topics are categories that are used to organize and classify different types of customer inquiries or issues. Help topics can be used to help customers find the appropriate resources or assistance for their specific needs, and can also help support staff efficiently route and prioritize incoming requests.

Add the following through:

    Admin Panel -> Manage -> Help Topics
  
    Business Critical Outage
  
    Personal Computer Issues
    
    Equipment Request
    
    Password Reset


</p>
<br />

