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

  
![image](https://github.com/user-attachments/assets/2fb92f73-b56a-45db-9e6a-e131cf3ee585)

![image](https://github.com/user-attachments/assets/7491dae3-b6bf-49b0-a21b-3b6b8d492b89)

![image](https://github.com/user-attachments/assets/2ce04afe-8bf3-4c7b-a3ee-158e992ab314)



Step 2: Configure Departments

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Departments
- Click 'Add New Department'
- In the name field enter System Administrators'
- Click 'Create Dept' at the bottom of the webpage



![image](https://github.com/user-attachments/assets/49e9bab0-2b14-45a9-b0cf-1ff8b488d643)

![image](https://github.com/user-attachments/assets/ac231d2f-5b02-4275-9c7f-0324a5e2603d)



Step 3: Configure Teams

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Agents -> Teams
- Click 'Add New Team'
- In the name field enter 'Level II Support' (Note: There should already be a 'Level I Support' team there)
- Click the 'Members' tab and add yourself to the team
- Click 'Create Team' at the bottom of the webpage


![image](https://github.com/user-attachments/assets/d28f74ad-58db-413e-8402-e93a2fcf6f49)

![image](https://github.com/user-attachments/assets/df3b1a82-c5a3-4e5e-b09a-bf4855d7e560)

![image](https://github.com/user-attachments/assets/7b2ac68d-637b-4250-85d3-826ae95e4d33)



Step 4: Configure to allow anyone to create tickets

-  Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Settings -> Users -> Settings
-  Make sure the 'Require registration and login to create tickets' box is unchecked

![image](https://github.com/user-attachments/assets/742c1679-29e7-4447-9631-d7a18db02ca0)



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


![image](https://github.com/user-attachments/assets/bfbb3a92-817a-446b-8937-d7d4d27e99d6)

![image](https://github.com/user-attachments/assets/210b9078-e85c-4745-87dd-f2c87eea5606)

![image](https://github.com/user-attachments/assets/d5246039-2453-4d77-a982-e2d4542e6551)

![image](https://github.com/user-attachments/assets/b1e90232-6b48-4d12-b86e-5fe3314c5f9a)

![image](https://github.com/user-attachments/assets/4d279b7f-f5d5-4110-965a-3c06e5064a28)



Step 6: Configure Users (Customers)

- Switch to the Agent Panel (top right should say Admin Panel, which means you're in the 'Agent Panel') -> Users -> Add User
- Enter a made up email address and name -> Add User
- Go back to the 'User Directory' and add a second user by repeating the exact same steps


![image](https://github.com/user-attachments/assets/886a04bf-09b0-4511-83f7-b38928a98bc9)

![image](https://github.com/user-attachments/assets/077eafe1-b0be-468f-9b3c-ca56e1e141c1)

![image](https://github.com/user-attachments/assets/ecdc862c-8663-4563-bd8a-6b81b52f755c)



Step 7: Configure SLA

- Switch back to the Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel')  -> Manage -> SLA
- Click 'Add New SLA Plan'
- Add SEV-A (Grace Period: 1 hour) (Schedule: 24/7)
- Add SEV-B (Grace Period: 4 hours) (Schedule: 24/7)
- Add SEV-C (Grace Period: 8 hours) (Schedule: Business Hours M-F)
- Click 'Add Plam' at the bottom of the webpage

![image](https://github.com/user-attachments/assets/1483c1b6-757c-4f88-bc81-df8bb8498dc9)

![image](https://github.com/user-attachments/assets/befdf785-ef24-4d3b-813c-ef37d594b809)

![image](https://github.com/user-attachments/assets/2de95311-a155-4016-835e-00cc14ef1a5a)



Step 8: Configure Help Topics

- Ensure you're under Admin Panel (top right should say Agent Panel, which means you're in the 'Admin Panel') -> Manage -> Help Topics
- Click 'Add New Help Topic'
- The following topics:
    - Business Critical Outage
    - Personal Computer Issues
    - Password Reset

![image](https://github.com/user-attachments/assets/a3bf6eb4-e9e9-41d3-8913-8a51270d7f55)

![image](https://github.com/user-attachments/assets/d437249a-eb18-4acf-b4f1-bb3682d9ed16)

![image](https://github.com/user-attachments/assets/9f5b3278-e1c9-48aa-8a85-8782e50daa9e)

![image](https://github.com/user-attachments/assets/05810ebc-87ef-4ebf-b430-d0903f0170bb)

![image](https://github.com/user-attachments/assets/4d707605-cf6f-481f-9b6d-bca66015f32e)
