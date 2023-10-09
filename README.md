<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />





<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>


-  PHP Manager 
-  Rewrite Module
-  PHP 7.3.8
-  VC_redist.86.exe
-  MYSQL 5.5.62
- Download and install osTicket 




<h2>Installation Steps</h2>

<p>



</p>
<p>
To start you must enable IIS in Windows With CGI.  Press start on the windows tab, and go to control panel.  Click on programs, then go to "Turn Windows features on or off" and navigate to Worle Wide Web Services -> Application Develoment Features -> Enable CGI, Common HTTP Features.  Also Enable IIS Management Console - Internet INformation Services ->Web managment Tool -> IIS Managment Console -> enable IIS MANAGMENT CONSOLE
</p>
<br />

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/7eeb5cfb-6ac6-419e-bbb2-05b32863520e)![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/4730b958-c668-4d97-98f1-a3b025c366ad)![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/c3bb14fc-c4d4-4bd3-8b5a-59cfbc73e336)




<p>



</p>
<p>
Download the following files.  On MYSQL download choose Typical Setup -> Launch Configuration Wizard -> Standard Configuration -> (Choose a Password)
After Register PHP from within IIS
</p>
<br />


<p>

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/24362059-3597-4264-86aa-e1ccc61fba63)
![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/6dba7c20-fd79-4c49-a61d-b31462c8d6b9)

</p>
<br />
Next Open up IIS, double click on PHP Manager -> Register new PHP version -> browse to C-drive -> PHP -> php-cgi- then execute

<p>


![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/51f27ae8-d5d3-450e-872e-07a18aea36aa)








</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
