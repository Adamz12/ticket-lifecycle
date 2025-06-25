<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>
<p>
First, navigate to the End-User portal at http://localhost/osTicket and click Open New Ticket
</p>
<p>
<img src="https://i.imgur.com/HC3GPBW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
- Enter a valid Email Address (e.g., karen@gmail.com)

- Select a Help Topic (e.g., Business Critical Outage)

- Enter a clear Subject (for example: “Entire mobile/online banking system is down”)

- Fill in a detailed Message describing the issue
 Finally, click Submit. You should see a confirmation with your new ticket number.
</p>
<br />

<p>
<img src="https://i.imgur.com/RbLAWmS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- Open your browser and go to the Admin/Analyst portal: http://localhost/osTicket/scp/login.php

- Log in using John’s credentials (username: john, password: Password1)

- Locate and click the ticket titled “Entire mobile/online banking system is down”

- In the Priority dropdown, select Sev-A and enter a comment like “Critical service outage – immediate attention required”

- In the Help Topic field, confirm or change to Business Critical Outage and add a note such as “Affecting all online banking users”

- For Department, choose Online Banking

- Under Assign To, select Jane (who’s in the Online Banking team)

- Click Save Changes to apply your updates
</p>
<br />

<p>
<img src="https://i.imgur.com/T6NJbZh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

- If John cannot modify the ticket, click Logout in the top-right corner

- Log back in at http://localhost/osTicket/scp/login.php with your Supreme Admin account (e.g., your-admin-username)

- In the Admin Panel, go to Agents → Agents

- Locate John and click Edit

- Change his Role from View Only to a role with broader access (e.g., Agent or Supreme Admin)

- Click Save Changes

- Log out of the Supreme Admin account and log back in as John—he should now be able to configure the ticket.
</p>
<p>
<img src="https://i.postimg.cc/Bv0ZsPZv/changing-john-settings.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
