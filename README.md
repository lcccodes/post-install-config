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
- Part 3: Add and configure users <b>**this uses the Agent Panel</b>
- Part 4: Configure SLAs (service level agreements) and Help Topics
  
<h2>Navigation and Configuration</h2>

<b>Part 1: Creating and observing A-records</b>

<p>
Creating roles, departments, teams and agents uses the same, very simple, navigation process:
<b>ADMIN PANEL > Agents tab > "Roles" (or "Departments" or "Teams")</b>

![image](https://github.com/lcccodes/post-install-config/assets/171904823/aea394d9-726b-4bfe-9f6d-38a81a3c9902)



</p>
<p>
Below: Once you define a role, click on the "Permissions" tab to choose among these options.

  ![image](https://github.com/lcccodes/post-install-config/assets/171904823/f71c6d7e-47e5-49ae-ab98-6fe5f01f4431)



</p>
<br />


<b>Part 2: About the local DNS cache</b>
<p>

![image](https://github.com/lcccodes/dnsconfig/assets/171904823/1dd7fe21-9c98-4103-ac6b-3385b826f481)


</p>
<p>
To see what's in your local DNS cache, use the command line interface (CLI) and type <b>ipconfig /displaydns</b>. If you suspect that the IP of a resource on the network may have changed, you might want to clear your cache using <b>ipconfig /flushdns</b>. This is harmless to do and it will just mean that your computer will need to consult for a brand new DNS record the next time it wants to call up a specific address. 
</p>
<br />


<b>Part 3: Creating a CNAME record</b>
<p>

![image](https://github.com/lcccodes/dnsconfig/assets/171904823/69e8d3fe-4e0d-4542-8114-76422d439455)


</p>
<p>
[ABOVE]: Similar navigation process as for creating or modifying an A-record. Right-click within the window and scroll down to create a new alias/CNAME. As you might expect with the concept of "alias," all that a CNAME does is convert one name to another name. So you could make a link to Wikipedia by using the name "learn" (although it wouldn't actually resolve).
</p>



<b>Part 4: Where to Find Root Hints within Server Manager</b>
</p>
<p>
  
![image](https://github.com/lcccodes/dnsconfig/assets/171904823/403e47d5-61a8-496c-a2c8-d15fa5bf1c68)



</p>
<p>
Root hints allow the DNS to resolve names and addresses that aren't yet in the cache. In Server Manager, you can reach this page from the same Tools menu in the upper right, then click on DNS, then your domain controller and right click "Properties" and find the Root Hints tab.
</p>
<br />
