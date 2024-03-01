<h1>Corrupted profile rebuild</h1>

 

<h2>Description</h2>
In this project i explain the process of rebuilding a corropted windows profile and transffering important files to  the new profile. 
<br />


<h2>Utilities Used</h2>

- <b>Windows Registry</b> 
- <b>File Explorer</b>
- <b>Control Panel</b>

<h2>Environments Used </h2>

- <b>Virtual Box</b> (21H2)
- <b>Windows 10 pro</b> (21H2)
- <b></b> (21H2)

<h2>Program walk-through:</h2>

log onto the clients computer with administrative account.
<img src="images/1.png" height="80%" width="80%"/>

Go into the c drive go to users find the affected profile and change the name to old.
<img src="images/change.old.png" height="80%" width="80%"/>

Go to the windows registry by typing run and regedit.
<img src="images/3.png" height="80%" width="80%" />

Go to local system, software, microsoft, windows nt, current version, profile list.
<img src="images/4.png" height="80%" width="80%" />

Next find the security identifier and export it to your desktop and delete the key in the registy.
<img src="images/5.png" height="80%" width="80%" />
 
 Next log out of the administrator acount and, log back in the the  users account.Windows will rebuild the profile
<img src="images/6.png" height="80%" width="80%" />
  
  <!--Windows will rebuid the profile.
<img src="images/.png" height="80%" width="80%" /> -->
  
  After the account is rebuilt log in with admin account and,find the old user account in the c drive.
<img src="images/7.png" height="80%" width="80%" or trianglead />
  
  Transfer needed files to the new user profile.
<img src="images/8.png" height="80%" width="80%" />
  
  Finaly log back into the user profile.
<img src="images/9.png" height="80%" width="80%" />

