<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Configuration </h1>
This tutorial will guide you through the process of configuring a simple ticketing system. The system includes roles, departments, teams, user settings, agents, users, SLAs (Service Level Agreements), and help topics. The configuration is outlined below.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents and Users
- Configure SLA and Help Topics

<h2>Configuration Steps</h2>

1. Configure Roles
    - Navigate to the Admin Panel.
    - Go to Agents -> Roles.
    - Add a role named "Admin."
    - Check off all permissions to give the role the ability to do everything.
      
      ![2](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/21e4d30d-1ccf-4414-9c08-3d814c42c120)
      ![1](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/204207f6-6906-455a-9720-e87a3792158b)

2. Configure Departments
    - In the Admin Panel, go to Agents -> Departments.
    - Add a new department named "System Administrators."
      
      ![4](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/8b972e76-d199-4645-be82-d168a2f209b2)
      ![3](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/bc2fc9b7-50ef-4880-be0d-d3c822ccf2b1)

3. Configure Teams
    - In the Admin Panel, navigate to Agents -> Teams.
    - Add two teams: "Level I Support"(if not already there) and "Level II Support."
  
      ![5](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/b833a7f6-1540-45a8-a240-a9eb1347b607)
      ![6](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/4af7ef77-24a9-40d9-ba07-a52fa18a9699)

4. Allow anyone to create tickets
    - Go to Admin Panel -> Settings -> User Settings.
    - Enable the option to "Require registration and login to create tickets."

      ![7](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/b9964433-b47b-4087-a7f5-17ac942dfee9)

5. Configure Agents (workers)
    - Visit Admin Panel -> Agents -> Add New.
    - Create an agent with the "Admin" role.
    - Create another agent with the ability to "Assign + Reply" only.
        - Primary Department > Role > Add new > Set permissions to Assign Tickets/Tasks and Reply to Tickets/Tasks only(this is for tutorial variation only, you can set it up to best fit your own needs)

       ** **BE SURE TO CREATE THE AGENT EMAIL ADDRESSES USING THE SAME EMAIL DOMAIN YOU CREATED IN STEP 14 OF THE [osTicket Installation Tutorial](https://github.com/mehmhacimic/osTicket-installation)** **    
      
      ![8](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/05419a12-ba8c-47c3-91b9-7705937de57b)
      ![9](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/e74c2d22-2aaf-4942-8f2c-e635fa6f841d)
      ![10](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/fea43036-ee48-411f-b3cc-5e391657d5e6)
      ![11](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/a243e47c-474f-4f5f-a3dc-6bf49f63f262)

6. Configure Users (customers)
    - Go to Agent Panel -> Users -> Add New.
    - Create two users with names of your choice.

      ![12](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/9af61ae2-5bb9-45ac-90f7-9b068e4882ea)
      ![13](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/3a78553f-d569-4fb9-90eb-5f17f7cba443)

7. Configure SLA
    - In Admin Panel -> Manage -> SLA.
    - Create the following SLAs:
        - Sev-A (Grace period: 1 hour, Schedule: 24/7)
        - Sev-B (Grace period: 4 hours, Schedule: 24/7)
        - Sev-C (Grace period: 8 hours, Schedule: M-F, business hours)
     
      ![14](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/879cf766-07a0-43fe-9454-2630c01a8819)
      ![15](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/0298503e-a16b-42c0-aab8-69f756c21794)

8. Configure Help Topics
    - Navigate to Admin Panel -> Manage -> Help Topics.
    - Add the following help topics: 
        - Business Critical Outage (Sev-A)
        - PC Issues (Sev-B)
        - Equipment Request (Sev-B)
        - Password Reset (Sev C)
  
      **  **Priority is not as important for this lab, just label each Help Topic whatever you think fits best** **

      ![16](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/62e22e26-3704-4b8b-853c-59338fbe8c46)
      ![17](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/509463d7-3e47-45c9-b5b2-bf6e066df030)
      ![19](https://github.com/mehmhacimic/osTicket-Configuration/assets/157438082/631ef0d7-cea2-4a78-9cf5-7f8b368808eb)


   

      


Congratulations! You have successfully configured a simple ticketing system. Feel free to customize the system further based on your specific requirements. 
If you have any questions or need additional assistance, refer to the documentation of your ticketing system or reach out to me via [LinkedIn](https://www.linkedin.com/in/mehmedalijahacimic/)/email for support.






