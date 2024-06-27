<h1>What to Configure Once You've Installed osTicket </h1>
This is just a few basics, partly so I remember certain details.
<p></p>
A key point is to always keep in mind whether you're working on the "admin panel" or the "agent panel." You can discern this by reading the link available in the upper right of the console. If it invites you to click on the "agent panel," that means you're currently on the "admin panel." (Admins can perform setup tasks, define roles and SLAs; while agents can open/close tickets and related tasks). The large majority of what follows below are system-administrator tasks that are performed on the admin panel.
<br />


<h2>Environments, Technologies and Languages Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop connections to a server and client
- osTicket


<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (22H2)

<h2>Overview</h2>

- Part 1: Configure Roles, Departments, Teams (if needed) and Agents
- Part 2: Ensure anyone can create tickets
- Part 3: Add and configure users <i>**this uses the Agent Panel</i>
- Part 4: Configure SLAs (service level agreements) and Help Topics
  
<h2>Navigation and Configuration</h2>

<b>Part 1: Configure Roles, Departments, Teams, Agents</b>

<p>
Creating roles, departments, teams and agents uses the same, very simple, navigation process:
<p></p>
<b>ADMIN PANEL > Agents tab > "Roles" (or "Departments" or "Teams") and "ADD NEW"</b>
<p></p>

![image](https://github.com/lcccodes/post-install-config/assets/171904823/aea394d9-726b-4bfe-9f6d-38a81a3c9902)



</p>
<p>
Above: note the separate section for "Agents" that is itself on the Agents tab. 
<p></p>
Below: Once you define a role, click on the "Permissions" tab to choose among these options.
<p></p>

  ![image](https://github.com/lcccodes/post-install-config/assets/171904823/f71c6d7e-47e5-49ae-ab98-6fe5f01f4431)



</p>
<br />


<b>Part 2: Ensure Anyone Can Create Tickets</b>
<p>

  ![image](https://github.com/lcccodes/post-install-config/assets/171904823/a0fcf64d-1330-4fb0-be55-6fe64446ed2a)



</p>
<p>
Make sure the highlighted box (ABOVE) remains unchecked. 
</p>
<br />


<b>Part 3: Add and configure Users </b>
<p>
<p></p>
For this step, make sure you've toggled onto the Agent panel (in upper right).
<p></p>

![image](https://github.com/lcccodes/post-install-config/assets/171904823/fdd31355-1a39-4ac6-a24b-ec20f0100f67)



</p>
<p>
[ABOVE]: Very simple navigation. In this photo, in the upper right, you can see the link to the "Admin panel," which indicates that you're currently on the Agent panel.
</p>



<b>Part 4: Configure SLAs and Help Desk Topics</b>
</p>
Navigation is the same for doing each of these:
ADMIN PANEL > Manage tab > "SLAs" (or "HelpTopics")
<p>
  
![image](https://github.com/lcccodes/post-install-config/assets/171904823/d2e64fa5-1b10-47ac-896e-aa3c297f36d9)




</p>
<p>
Root hints allow the DNS to resolve names and addresses that aren't yet in the cache. In Server Manager, you can reach this page from the same Tools menu in the upper right, then click on DNS, then your domain controller and right click "Properties" and find the Root Hints tab.
</p>
<br />
