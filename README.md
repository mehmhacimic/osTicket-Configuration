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

        **BE SURE TO CREATE THE AGENT EMAIL ADDRESSES USING THE SAME EMAIL DOMAIN YOU CREATED IN STEP 14 OF THE [osTicket Installation Tutorial](https://github.com/mehmhacimic/osTicket-installation)**

6. Configure Users (customers)
    - Go to Agent Panel -> Users -> Add New.
    - Create two users with names of your choice.

7. Configure SLA
    - In Admin Panel -> Manage -> SLA.
    - Create the following SLAs:
        - Sev-A (1 hour, 24/7)
        - Sev-B (4 hours, 24/7)
        - Sev-C (8 hours, business hours)

8. Configure Help Topics
    - Navigate to Admin Panel -> Manage -> Help Topics.
    - Add the following help topics:
        - Business Critical Outage (Sev-A)
        - PC Issues (Sev-B)
        - Equipment Request (Sev-B)
        - Password Reset (Sev C)


Congratulations! You have successfully configured a simple ticketing system. Feel free to customize the system further based on your specific requirements.
