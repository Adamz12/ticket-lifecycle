<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


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
<img src="https://i.postimg.cc/3x45kNcd/support-center.png" height="800" width="800" alt="Disk Sanitization Steps"/>
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
<img src="https://i.postimg.cc/KzQsqhH6/creating-1st-ticket.png" height="800" width="800" alt="Disk Sanitization Steps"/>
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
<img src="https://i.postimg.cc/N0dzbwVW/editing-ticket.png" height="800" width="800" alt="Disk Sanitization Steps"/>
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
<img src="https://i.postimg.cc/Bv0ZsPZv/changing-john-settings.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>
<p>

- Open your browser and go to the Admin/Analyst portal: http://localhost/osTicket/scp/login.php

- Log in with Jane’s credentials (username: jane, password: Password1)

- Find and open the ticket “Entire mobile/online banking system is down”

- Change Status to In Progress

- In the Public Reply box, enter:

- We suspect the recent system updates caused this outage. We’ll roll back those updates shortly and investigate further.

- Click Post Reply to notify the requester

- (Later, after investigating and rolling back updates) open the ticket again

- Change Status to Resolved

- In the Public Reply box, enter:

- The issue was confirmed to be with the updates. We’ve rolled them back, notified the vendor, and online banking services are now back up.

- Click Post Reply and then Close Ticket to complete the workflow
</p>
<p>
<img src="https://i.postimg.cc/vTV512ky/work-ticket-A-as-jane.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.postimg.cc/7ZWPcPbB/ticket-A-resolved.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>

<p>

- Open your browser and go to the End-User portal: http://localhost/osTicket

- Click Open New Ticket

- Enter Email: ken@gmail.com

- Select Help Topic: General Enquiry

- In Subject, type: “Accounting department needs Adobe update”

- In Message, type: “The accounting department cannot use the Adobe software.”

- Click Submit to create the ticket.
</p>
<p>
<img src="https://i.postimg.cc/5yRkJrvM/create-ticket-B.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>

<p>

- Open the Admin/Analyst portal (http://localhost/osTicket/scp/login.php) and log in as John

- Locate and open the “Accounting department needs Adobe update” ticket

- In the Assign To field, select John

- Change Priority to Sev-C (lower urgency for two users affected)

- Click Post Reply with:

- Please restart your computers and let us know if the issue persists.

- After the restart confirms the issue is resolved, click Post Reply with:

- Restarting the machines has resolved the problem. Closing the ticket now—feel free to reopen if anything else comes up.

- Change Status to Closed to complete the ticket lifecycle.
</p>
<p>
<img src="https://i.postimg.cc/3N4zk73w/Working-ticket-B.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>

<p>

- Open your browser and go to the End-User portal: http://localhost/osTicket

- Click Open New Ticket

- Enter Email: karen@gmail.com

- Select Help Topic: Personal Computer Issues

- In Subject, type: “CFO’s laptop will not turn on”

- In Message, type: “The laptop will not turn on, even though the power button is being pressed.”

- Click Submit to create the ticket.
</p>
<p>
<img src="https://i.postimg.cc/xdzfN6kD/creating-ticket-C.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>

<p>

- Open the Admin/Analyst portal (http://localhost/osTicket/scp/login.php) and log in as John

- Locate and open the “CFO’s laptop will not turn on” ticket

- Change Priority to Sev-B

- Set Department to Support

- In Assign To, select John

- Click Post Reply with:

- After investigating, we found the charger wasn’t working. Once the charger was replaced, the laptop powered on normally.

- Change Status to Closed to mark the ticket as resolved.
</p>
<p>
<img src="https://i.postimg.cc/XJnvMwvR/working-ticket-C.png" height="800" width="800" alt="Disk Sanitization Steps"/>
</p>

<h2>Conclusion</h2>
<p>
And that wraps up our osTicket lab—from setting up the VM and installing all components to managing tickets through their full lifecycle. Don’t forget to shut down your VM when you’re done to save costs, or delete the resource group if you’re finished with the entire environment. Thank you for following along!
</p>
<br />
