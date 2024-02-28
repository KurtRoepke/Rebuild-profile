<h1>Corrupted file rebuild</h1>

 

<h2>Description</h2>
This project explain's the process of creating an instance of windows server 2022 and, a windows 10 pro client. The project also explains creating an active directory domain with an admin ou and, account. Finaly the project also explains setting up basic nat/routing, dhcp server and, a dns server. 
<br />


<h2>Utilities Used</h2>

- <b>Server manager</b> 
- <b>Cmd</b>
- <b>Control Panel</b>

<h2>Environments Used </h2>

- <b>Virtual Box</b> (21H2)
- <b>Windows 10 pro</b> (21H2)
- <b>Windows Server 2022</b> (21H2)

<h2>Program walk-through:</h2>

Create a virtual machine in virtualbox and select windows server 2022 for desktop.
<img src="createDC.png" height="80%" width="80%"/>

Add two nic's one with nat and, one internal nic for client pc.
<img src="addNic.png" height="80%" width="80%"/>

Go to control panel, system, rename pc(advanced) change pc name to DC and add to domain.
<img src="dmchange.png" height="80%" width="80%" />

Go to network and sharing center choose network connections label both nic's and, add defult gateway.
<img src="nic.png" height="80%" width="80%" />

Go to server manager and select add roles.
<img src="addroles.png" height="80%" width="80%" />
 
 Select the domain controller.
<img src="selectserver.png" height="80%" width="80%" />
  
  Choose active directory domain services and, click next and install.
<img src="dhcp.png" height="80%" width="80%" />
  
  Go to the yellow triangle to create a new domain. 
<img src="trianglead.png" height="80%" width="80%" or trianglead />
  
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


