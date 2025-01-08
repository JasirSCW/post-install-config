<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)



<h2>Configuration Steps</h2>

![OsTicket1](https://github.com/user-attachments/assets/064f425e-280e-40ba-be79-7121610d4477)

![Osticket2](https://github.com/user-attachments/assets/6af5433b-c2ea-4225-9e55-98c44a7f9063)

After installing osTicket, it's time to configure it for use as a ticketing system. Keep in mind that the Admin and Agent panels have distinct settings, so I'll need to switch between them based on what needs to be configured. To determine which panel I'm using, I can check the top-right corner of the screen. If it says "Agent Panel," I'm in the Admin panel, and vice versa.

The first configuration step is to create a new role called Supreme Admin. This role will have all available permissions for this lab's purposes. To set this up, I'll go to the Admin panel, navigate to the Agents menu, and click on Roles. From there, I'll create the new role and assign it full permissions.




</p>
<p>

</p>
<br />


![OsTicket3](https://github.com/user-attachments/assets/a2e9ba96-5e4f-43db-ba51-24330607b43f)

The next step is to create a new Department specifically for System Administrators. To do this, I'll navigate to the Admin panel, open the Agents menu, and select Departments. From there, I can add a new Department and name it "System Administrators" to organize and manage tickets efficiently.


![OsTicket4](https://github.com/user-attachments/assets/8e95c12b-17bc-40d6-a925-e5b2216c585b)

The next step is to create a new Online Banking Team to complement the existing Level I Support Team in osTicket. To do this, I'll go to the Admin panel, open the Agents menu, and select Teams. From there, I can add the new team by naming it "Online Banking Team" and configure it as needed to support the ticketing workflow.

![OsTicket5](https://github.com/user-attachments/assets/e1e19746-7243-4f30-bd42-bc347d5ae634)

</p>
<p>To ensure tickets in the queue are handled, new agents need to be created. I'll navigate to the Admin panel, open the Agents menu, and click on Add New Agent. From there, I'll set up the account credentials for each new agent. For this example, I'll create accounts for Jane Doe and John Doe.
</p>
<br />

![OsTicket6](https://github.com/user-attachments/assets/056abfa7-3117-463a-bb80-a6eaef1e5c15)

To allow ticket creation for agents to triage, new users need to be added. I'll switch to the Agent panel, open the Users menu, and click on Add User. From there, I'll create the necessary account credentials. For this example, I'll set up accounts for Karen.

![OsTicket7](https://github.com/user-attachments/assets/a7a577d0-f2f1-4fff-acfb-f43c3e2d6019)

To categorize tickets based on their level of impact, Service Level Agreements (SLAs) need to be created. I'll go to the Admin panel, open the Manage menu, and select SLA. From there, I'll create the necessary SLAs. For this setup, I'll create the following:

SEV-A: Tickets requiring resolution within 1 hour.
SEV-B: Tickets requiring resolution within 4 hours.
SEV-C: Tickets requiring resolution within 8 hours.

![osTicket8](https://github.com/user-attachments/assets/0d9a5811-7c05-430d-ac6e-38dc9bdd6833)

The final step is to create Help Topics to guide users in categorizing their issues, giving agents a clearer understanding of the problems described in tickets. To do this, I'll go to the Admin panel, open the Manage menu, and select Help Topics. Then, I'll click on Add New Help Topic and create the following categories for use in future tickets:

Business Critical Outage
Personal Computer Issues
Equipment Reset
Password Request

<h1>osTicket - Configurations are Complete</h1>
Now that I've completed the osTicket configurations, I can fully utilize it as a proper ticketing system. I can create tickets and triage them just like I would in a real environment. This setup will help me stay organized and efficiently manage support issues. If I want to optimize the process further, I could explore additional features like automating ticket assignments, setting up email notifications, or customizing user roles.
