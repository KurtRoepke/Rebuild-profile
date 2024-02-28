<h1>Corrupted profile rebuild</h1>

 

<h2>Description</h2>
In this project i explain the process of rebuilding a corropted windows profile and transffering important files to  the new profile. 
<br />


<h2>Utilities Used</h2>

- <b></b> 
- <b></b>
- <b>Control Panel</b>

<h2>Environments Used </h2>

- <b>Virtual Box</b> (21H2)
- <b>Windows 10 pro</b> (21H2)
- <b></b> (21H2)

<h2>Program walk-through:</h2>

log onto the clients computer with administrative account.
<img src="images/.png" height="80%" width="80%"/>

Go into the c drive go to users find the affected profile and change the name to old.
<img src="images/.png" height="80%" width="80%"/>

Go to the windows registry by typing run and regedit.
<img src="images/.png" height="80%" width="80%" />

Go to local system, 
<img src="images/.png" height="80%" width="80%" />

Next export the user profile to your desktop and delete the key in the registy.
<img src="images/.png" height="80%" width="80%" />
 
 Next log out of the administrator acount and, log back in the the  users account.
<img src="images/.png" height="80%" width="80%" />
  
  Windows will rebuid the profile.
<img src="images/.png" height="80%" width="80%" />
  
  After the account is rebuilt log in with admin account and,find the old user account.!!
<img src="images/.png" height="80%" width="80%" or trianglead />
  
  Go to tools then active directory users and computers and, create new administrator ou.
<img src="Newou.png" height="80%" width="80%" />
  
  Next create a new admin user.
<img src="1.png" height="80%" width="80%" />

  Go to user properties and, add to admin group log out then log back in with the admin account.
<img src="newpic.png" height="80%" width="80%" />

Go to add roles and select routing.
<img src="routing.png" height="80%" width="80%" />

 Select routing and install.
<img src="3.png" height="80%" width="80%" />
 
 Next select tools, routing an remote, choose nat and choose the external nic.
<img src="4.png" height="80%" width="80%"  />

 Go to add roles and, select dhcp click next and install.
<img src="dhcpc.png" height="80%" width="80%" />

Select tools then select dhcp and, right click ipv4 next select new scope.
<img src="scope.png" height="80%" width="80%" />

 Next add router with defult gateway.
<img src="addr.png" height="80%" width="80%" />

 Go to the yellow triangle and press dhcp to authorize the dhcp server.
<img src=" 5.png " height="80%" width="80%" />

 Install a client windows 10 pro virtual machine.
<img src="6" height="80%" width="80%" />

 Next go to change computer name and join mydomain.com.
<img src="7.png" height="80%" width="80%" />

 Finaly to confirm connectivity ping the defult gateway and then an outside ip address. 
<img src="8.png" height="80%" width="80%" "/>


