<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (Windows App)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

![Screen Shot 2024-12-28 at 10 50 01 AM](https://github.com/user-attachments/assets/96faf6e5-dc6e-41c4-ae81-0c769135835a)

First, we'll start by configuring the roles. Admin Panel > Agents > Roles > Add New Role. Name it "Supreme Admin".
</p>
<br />

![Screen Shot 2024-12-28 at 10 52 18 AM](https://github.com/user-attachments/assets/98bd7b97-0977-4417-b4eb-44431cda74de)

![Screen Shot 2024-12-28 at 10 52 46 AM](https://github.com/user-attachments/assets/90466358-3316-4956-b304-abe2bd9ac497)

![Screen Shot 2024-12-28 at 10 53 08 AM](https://github.com/user-attachments/assets/7c2d79ef-5657-47fd-8847-2c382dce781b)

![Screen Shot 2024-12-28 at 10 57 20 AM](https://github.com/user-attachments/assets/47422e65-ed64-49ff-9612-2aa714856b79)

Go to Permissions and check all the boxes under Tickets, Tasks, and Knowledgebase to assign the Supreme Admin full control. Add the new role.
</p>
<br />

![Screen Shot 2024-12-28 at 11 01 39 AM](https://github.com/user-attachments/assets/659ad189-a5a5-4d5e-b4f2-ec1623f30289)

Next, we'll configure the departments. Admin Panel > Agents > Departments > Add New Department. Name it "SysAdmins".
</p>
<br />

![Screen Shot 2024-12-28 at 11 06 29 AM](https://github.com/user-attachments/assets/5fed5888-649b-4736-97cd-6228132080ea)

Now we'll configure the teams. Admin Panel > Agents > Teams > Add New Team > Name it "Online Banking" > Create Team.
</p>
<br />

![Screen Shot 2024-12-28 at 11 12 17 AM](https://github.com/user-attachments/assets/9a91e8fa-9d69-4a14-9d19-f38122d6a02a)

We're now going to change the settings to allow anyone to create a ticket. This is so that end users that may not have registered in the system may create tickets. Admin Panel > Settings > User Settings (UNCHECK: unregistered users can create tickets). Registration required: Require registration and login to create tickets.
</p>
<br />

![Screen Shot 2024-12-28 at 11 20 18 AM](https://github.com/user-attachments/assets/2506b73a-f688-4f85-9fdd-970910efa2ac)

Next, we'll configure agents (workers). Admin Panel > Agents > Add New Agent. Create the new agents as Jane (Dept. SysAdmins) and John (Dept. Support). Make note of the usernames and passwords you create for each agent.
</p>
<br />

![Screen Shot 2024-12-28 at 11 26 17 AM](https://github.com/user-attachments/assets/b1da2382-1954-40ca-b0a2-9f9375f2c943)

![Screen Shot 2024-12-28 at 11 26 32 AM](https://github.com/user-attachments/assets/4940be46-8699-4554-9920-12ab483f48e0)

For Jane:
</p>
<br />

![Screen Shot 2024-12-28 at 11 27 56 AM](https://github.com/user-attachments/assets/7941dda8-06a2-42b0-bc42-356a53b2d1aa)

For John:
</p>
<br />

![Screen Shot 2024-12-28 at 11 36 43 AM](https://github.com/user-attachments/assets/c5a181c9-2c3a-4185-bc9b-955d9c6f1ec2)

We will configure the Users now. Agent Panel > Users > Add User. Add Karen.
</p>
<br />

![Screen Shot 2024-12-28 at 11 46 02 AM](https://github.com/user-attachments/assets/6d5b96ff-e12a-4c04-9ac1-64e4a53afa03)

![Screen Shot 2024-12-28 at 11 47 29 AM](https://github.com/user-attachments/assets/3ddd8470-d4cd-4368-a2e6-8596b2913cf7)

![Screen Shot 2024-12-28 at 11 48 02 AM](https://github.com/user-attachments/assets/7bdf5fdf-a543-4973-814c-bd3254587a7b)

![Screen Shot 2024-12-28 at 11 48 34 AM](https://github.com/user-attachments/assets/b8de3b93-06d9-4d16-a3b7-3f4de0991f6c)


Next, configure SLA. Admin Panel > Manage > SLA > Add New SLA Plan. We will create 3 SLAs. Sev-A (Grace Period: 1 hour, Schedule: 24/7), Sev-B (Grace Period: 4 hours, Schedule: 24/7), Sev-C (Grace Period: 8 hours, Business Hours)

</p>
<br />

![Screen Shot 2024-12-28 at 11 53 37 AM](https://github.com/user-attachments/assets/0f6e1086-209a-4814-85f7-883e841ccba4)

![Screen Shot 2024-12-28 at 11 54 26 AM](https://github.com/user-attachments/assets/daa8d11a-7798-4595-9147-fd2d8c1b4b3f)

![Screen Shot 2024-12-28 at 11 55 13 AM](https://github.com/user-attachments/assets/bc981a49-cfe5-4cbf-b015-1e0f1b2ca183)

![Screen Shot 2024-12-28 at 11 55 40 AM](https://github.com/user-attachments/assets/7393dbe3-2593-469a-ae5b-98d8d04c6a81)

![Screen Shot 2024-12-28 at 11 56 06 AM](https://github.com/user-attachments/assets/eface9e6-960d-4ff4-ab17-394dc59a1e31)

Finally, we'll configure Help Topics. This is for when users create tickets. Admin Panel > Manage > Help Topics > Add New Help Topic. Create these new help topics: Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset, Other.

</p>
<br />

![Screen Shot 2024-12-28 at 11 56 54 AM](https://github.com/user-attachments/assets/5a4592e4-9f17-433a-b0f5-2bde6180d1ed)

This completes the full setup of osTicket. I hope this guide has been helpful in clarifying the process and assisting you in configuring your system. It’s highly recommended to practice ticket triaging and resolution.

These are essential skills for any help desk specialist, as they serve as the primary point of contact between a company and its customers when addressing product or service-related issues.
</p>
<br />

