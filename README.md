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
Now install osTicket.  Extract and copy "upload" folder to c:inetpup/wwwroot.  
  Reload IIS, then go to sites -> default ->osTicket -> on the right, click "Browse :80".  Go back to IIS, sites ->Default -> osTicket -> Double-click PHP Manager -> "Enable or disable an extension.  Enable the following (php_imap.dll, php_intl.dll, php_opache.dll) and refresh                                                                                                                                                                                                                                                                                     
  
  
</p>
<br />

</p>

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/cbbb5b04-acfa-4b88-8c8f-41bd887944ec)![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/12d35f36-86e9-4d3a-8381-69e396ec704b)




</p>
<p>
Now Rename:ost-config.php.  C:/inetpub\wwwroot\osTicket\include\ost-sampleconfig.php To:  C:/inetpub\wwwroot\osTicket\include\ost-config.  After renaming it give it permissions by righting clicking ost-config -> protperties -> Security -> Advanced -> Disable inheritance.  Then with New permission ->Everyone -> All

</p>
<br />

</p>

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/9b182de8-ed1d-4ff4-893e-d28ba1400fe5)


</p>
<p>

Go back to IIS and browse back to "Browse :80, and continue to setup osTicket.  When you get to my SQL database, open Heidi SQL -> riht click unamed -> Create a new session, make root password -> Connect to session -> Create a database called "osTicket".  Continue setting up osticket in browser with the credetials you created and press intall now. 

</p>
<br />

</p>

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/55e6b867-f95e-46e0-83ec-54035e17a375) ![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/b990a3e1-ad91-4946-a1a8-142ceb7143af)
 ![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/d0dedb3c-fc61-4a82-8ef8-49b5101669c1) ![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/742850e9-3e29-438c-bdbc-18abfb2f66e2)![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/5d3dd8f9-28d1-4a87-977c-3dc6289c82d4)

</p>
<p>

IF it looks like this then Congrats!!! 

</p>
<br />

</p>

![image](https://github.com/AtomSteve/osticket-prereqs/assets/147112183/5267d272-f991-4ecf-a70e-503689aa30a0)


