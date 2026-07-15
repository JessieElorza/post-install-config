# post-install-config
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Azure Storage
- Windows Server
- Remote Desktop Connection
- Internet Information Services (IIS)
- osTicket
- Windows 11

<h2>Operating Systems Used </h2>

- Windows 11 (Desktop)
- Windows 11</b> (25H2) (Virtual Machine)

<h2>Post-Install Configuration Objectives</h2>

- Creating Users and Agents. Setting up roles and permissions for the created users and agents
- Configure ticket visibility and help desk functionality.
- Configuring SLAs to define response times for tickets.
- Adding different types of help topics to enhance efficency and user experience.
- Enhance user experience by organizing help topics.

<h2>Configuration Steps</h2>

<p>
Once logged into osTicket switch to the Admin Panel then navigate to Agents -> Roles. Click Add New Role.
</p>
<p>
<img src="https://github.com/user-attachments/assets/c0a7decc-3359-4c2c-80bc-f9b557bbb75d" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/9467df74-300c-4e58-a5ff-c93adb513a82" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Name the new role "Supreme Admin" then in the permissions tab check every box for permissions/access. Create the Role. This allows full system control and configuration capabilities for an account with complete control over the help desk system. The Supreme Admin account acts as the primary system administrator that manages the system.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/6a348bc3-cd2e-4b5f-972e-1af8835dcda0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Agents -> Departments -> Add New Department. Switch the Parent to "Top-Level Department" and named the department "SysAdmins". Create the Department. Deparments are to ensure tickets are properly assisgned and accessible only to authorized agents.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/d02eeafd-eee8-4bb1-b61d-3a347d424d42" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Agents -> Teams -> Add New Team. Name it "Online Banking" then create the team. Teams are to support ticket escalation and coordinate issues to specific departments in a buisness.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/d9b1fc8b-daad-41d1-8be0-768799b19bb1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Settings -> Users. Verify that the "Registration Required:" setting is unchecked. This makes it so people aren't required to register and login to create a ticket. This allows ease of access and easy workflow for ticket creation for the sake of the client.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/7598a85c-7477-4e42-aac2-3232078817fd" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Agents -> Add New Agent. Created an agent called "Jane Doe" with the following credentials (Note: A fake email was used):
</p>
<p>
  -Name: Jane Doe
</p>
<p>
 -Email: jane@lognpacific.com
</p>
<p>
  -Username: jane
</p>
<p>
  -Password: Password1
</p>
<p>
<img src="https://github.com/user-attachments/assets/6b76fc02-12e3-4e83-9a5b-04c632fb570b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a2d4a07c-b688-43bd-b7da-ab3cad6f893e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Give Jane the "SysAdmin" Department with the Role of "Supreme Admin" so that agent can have complete access and control over the ticketing system. Add Jane to the "Online Banking" Team as well so the agent can be a part of the ongoing overseeing of issues in this department. This will allow her to see all tickets that come through the "Online Banking" Department.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/4c7ca692-0be7-4e57-be36-a2935740196a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/83768cb6-4585-4db3-bced-e32197801f90" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Agents -> Add New Agent. Created an agent called "Jane Doe" with the following credentials (Note: A fake email was used):
<p>
  -Name: John Doe
</p>
<p>
 -Email: john@lognpacific.com
</p>
<p>
  -Username: john
</p>
<p>
  -Password: Password1
</p>
<p>
Gave John the "Support" Department with the Role of "View Only" with limited controls. Create the agent.

Agent roles and departmental access to align with the defined ticket visibility and workflow structure.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/134a8e73-594d-4ac5-b489-8ceac7b472a9" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Accessed the Agent Panel.

Navigated to Users → Add New.

Created end-user accounts to simulate customer interaction within the help desk system:

Karen and Ken,
Configured user profiles to enable ticket submission and support request tracking through the osTicket portal.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/00bbd56b-1114-4bc0-81b5-ab3edec5042a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/f6eec205-08e9-403e-b675-304f658f7f5f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Manage -> SLA -> Add New SLA Plan. Created 3 different plans with the following:
</p>
<p>
 - Sev-A (1 hour, 24/7)
</p>
<p>
- Sev-B (4 hours, 24/7)
</p>
<p>
 - Sev-C (8 hours, Business Hours)
</p>
<p>
Service Level Agreements (SLAs) help define a severity of the problem and the resolution time expected based on the ticket severity. Ensures resources are allocated effectively and Critical issues (such as system outages) receive faster attention than lower-priority requests.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/f465b79f-d623-4d97-9fec-8df65b870fdb" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/6e9b859c-2075-4390-8a58-0d7aa3f421d3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel navigate to Manage -> Help Topics -> Add New Help Topic. Added the following Topics:
<p>
- Business Critical Outage (Report a problem)
</p>
<p>
- Persosnal Computer Issues (Report a problem)
</p>
<p>
- Equipment Request (General Inquiry)
</p>
<p>
- Password Reset (Report a problem)
</p>
<p>
- Other (General Inquiry)
</p>
<p>
Help Topics help align with SLA policies and enable structured prioitization for tickets. They categorize support requests and groups tickets by category, such as Technical Support, Billing, Sales, or General Inquiry and route tickets efficiently.
</p>
<br />

<h2></h2>

### End Of Project
This concludes the post-installation configuration of the osTicket environment. Through the implementation of role-based access control, departmental structuring, SLA policies, and categorized help topics, the system was configured to support efficient ticket management and a structured workflow for both support agents and end users and demonstrates knowledge and literacy in osTicket's basic functioning workflow systems in a workplace.
