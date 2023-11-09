<h1>Active Directory Lab with PowerShell</h1>

<h2>Description</h2>
This project establishes a Windows Server 2019 environment with Active Directory, DHCP, and Remote Access, streamlining user management and ensuring seamless connectivity. In a corporate setting, this infrastructure enhances efficiency, centralizes user administration, and promotes secure network management, fostering a well-organized and productive IT environment.
<br />


<h2>Resources Used</h2>

- <b>Active Directory</b> 
- <b>PowerShell</b>
- <b>Windows Server</b> 
- <b>Virtualization (Oracle VirtualBox)</b>

<h2>Project walk-through:</h2>

<p align="center">
Diagram Overview: <br/>
<img src="https://i.imgur.com/QuPTjLC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Installed & Configured Windows Server 2019 in Oracle VM Virtualbox:  <br/>
<img src="https://i.imgur.com/NOuGuEq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Identified Internal NIC, Configured IPv4 Address & DNS Settings:  <br/>
<img src="https://i.imgur.com/Ht7Y8iZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Added Active Directory Domain Services, Configured DC Options:  <br/>
<img src="https://i.imgur.com/zlBwafv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created OU for “Admins”, Created User Profile, & Added Domain Admins Group:  <br/>
<img src="https://i.imgur.com/qI7DjCp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Added Remote Access Role to Allow Private Virtual Network Connection Between CLIENT1 and DC and Ability to Access Internet When Using CLIENT1:  <br/>
<img src="https://i.imgur.com/iueLqOG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configured the Routing and Remote Access Settings on the DC: <br/>
<img src="https://i.imgur.com/ct8hZRW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Added DHCP Server Role, Added Scope of IP Addresses, Configured the Lease Duration, and Authorized the DHCP Server:  <br/>
<img src="https://i.imgur.com/K7LvUuX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Auto Added 1,000 Users with PowerShell ISE, Used a .TXT File with Auto Generated Names, Used the Following Script to Add them to AD under a “Users” OU:  <br/>
<img src="https://i.imgur.com/aDP7HAM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/wd5bOX7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Installed & Configured another VM with Windows 10 Pro, Checked IP Configuration (Successfully Assigned an IP Address within the Scope Configured), & also able to Ping Google’s DNS Server:  <br/>
<img src="https://i.imgur.com/E7ixqyC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Joined CLIENT1 to the Domain Successfully, Opened DHCP Management Console and Verified the IP Address that was Leased:  <br/>
<img src="https://i.imgur.com/AbxLFGM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
CLIENT1 was able to Access Internet:  <br/>
<img src="https://i.imgur.com/fkx6eTJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
