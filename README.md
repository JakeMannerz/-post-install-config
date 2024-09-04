<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)



<h2>Configuration Steps</h2>


Step 1: Configure Roles

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Roles -> Add New role
- Add Name (Supreme Admin)
- Click the 'Permissions' tab and Check all boxes under Tickets\Tasks\Knowledgebase
- Click Add Role

 ![image](https://github.com/user-attachments/assets/e1fa2ae8-5f25-4a2c-9498-ac4a546c88dd)

![image](https://github.com/user-attachments/assets/36e08e6e-f77e-4940-a474-bbbbd5b2208e)

![image](https://github.com/user-attachments/assets/bc94dc79-92e3-4fa4-af02-48ee4a4adb99)



Step 2: Configure Departments

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Departments
- Click 'Add New Department'
- In the name field enter System Administrators'
- Click 'Create Dept' at the bottom of the webpage



![image](https://github.com/user-attachments/assets/f2844acc-00a0-4591-882d-59aafe5e6199)


![image](https://github.com/user-attachments/assets/fa9602ca-e0ed-4064-83ea-7ddeb7a27fa4)



Step 3: Configure Teams

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Teams
- Click 'Add New Team'
- In the name field enter 'Level II Support' (Note: There should already be a 'Level I Support' team there)
- Click the 'Members' tab and add yourself to the team
- Click 'Create Team' at the bottom of the webpage


![image](https://github.com/user-attachments/assets/7a07fc37-c983-4060-a490-29879c709090)


![image](https://github.com/user-attachments/assets/62e143b0-5a6c-48ef-ba4d-592906b2d285)

![image](https://github.com/user-attachments/assets/f2155eb4-ab20-4999-a9c9-e5523dc4ac7b)




Step 4: Configure to allow anyone to create tickets

-  Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Settings -> Users -> Settings
-  Make sure the 'Require registration and login to create tickets' box is unchecked

![image](https://github.com/user-attachments/assets/4daa5f06-c84d-4a8e-8f82-d423a9a787cf)



Step 5: Configure Agents (Help Desk Professionals)

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Add New Agent
- Add Agents Name\ Email Address\ Username
- Click 'Set Password' and deselect 'Send the agent a password reset email'
- Enter the Password (create your own) -> deselect 'Require password change at next login' -> click 'set'
- Assgin the department for the agent by click the 'Access' tab
- Select the department and the role
- Add the agent to the 'Level II Support' team that was created under the teams tab
- Click 'Create'
- Repeat steps to add a second agent
- Assign the second agent to the 'Support' department and 'View only' role under the 'Access' tab


![image](https://github.com/user-attachments/assets/080c8c62-21c9-4a4f-a984-dc1ea0df3ea0)


![image](https://github.com/user-attachments/assets/c772a422-d116-407a-bef1-65758f1f8dd6)


![image](https://github.com/user-attachments/assets/dbc3838d-3556-401e-b06c-d8a3f9208edc)

![image](https://github.com/user-attachments/assets/41eb9895-e627-44fd-ac29-4a96abb5c5d0)

![image](https://github.com/user-attachments/assets/4237f6d3-4dde-4f70-997d-a5fd98cd1f82)

![image](https://github.com/user-attachments/assets/a20b5d4e-7027-4dcb-bab2-c6e1be5e1a57)




Step 6: Configure Users (Customers)

- Switch to the Agent Panel (top right should say Admin Panel, which means you're in the 'Agent Panel') -> Users -> Add User
- Enter a made up email address and name -> Add User
- Go back to the 'User Directory' and add a second user by repeating the exact same steps


![image](https://github.com/user-attachments/assets/2257f99f-7199-44cc-8c94-607dba442126)


![image](https://github.com/user-attachments/assets/d7d4583e-4b79-4060-8a0e-c3f20eec01bb)


![image](https://github.com/user-attachments/assets/f32a84f0-fea4-4d21-a1e6-ce170492de35)



Step 7: Configure SLA

- Switch back to the Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel')  -> Manage -> SLA
- Click 'Add New SLA Plan'
- Add SEV-A (Grace Period: 1 hour) (Schedule: 24/7)
- Add SEV-B (Grace Period: 4 hours) (Schedule: 24/7)
- Add SEV-C (Grace Period: 8 hours) (Schedule: Business Hours M-F)
- Click 'Add Plam' at the bottom of the webpage

![image](https://github.com/user-attachments/assets/d6d8bbdc-ac7f-4ce6-8251-1b490c0b574f)

![image](https://github.com/user-attachments/assets/86cbe6a6-38f7-42a2-adb0-898f2f9ed3d2)


![image](https://github.com/user-attachments/assets/08b2c7f6-d166-4bd4-aaf6-1e26651e02ba)




Step 8: Configure Help Topics

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage -> Help Topics
- Click 'Add New Help Topic'
- The following topics:
    - Business Critical Outage
    - Personal Computer Issues
    - Password Reset



![image](https://github.com/user-attachments/assets/043ab9cd-99af-4d28-a1dd-dc4576f7f0bf)


![image](https://github.com/user-attachments/assets/b6a5aa05-fda7-4b6d-9b91-e9d9617d2795)


![image](https://github.com/user-attachments/assets/51f7d4f8-7807-4441-913a-82e2ce98d8e9)


![image](https://github.com/user-attachments/assets/ef94fc8a-b3c0-4125-a6ee-c2bf3430bfdf)
![image](https://github.com/user-attachments/assets/05ef970e-c90b-4a45-9741-bf370ea0a2b5)

