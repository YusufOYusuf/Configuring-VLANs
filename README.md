<h1>Configuring VLANs</h1>


<h2>Description</h2>
In this lab, I learned to configure virtual local area networks (VLANs). VLANs are logical subdivisions of a switch that segregate ports from one another as if they were in different LANs. VLANs offer another way to add a layer of separation between sensitive devices and the rest of the network.
<br />



<h2>Environments Used </h2>

- <b>Ubuntu 20.04.2 LTS</b> 

<h2>Utilities and Language </h2>

- <b>PuTTY SSH Client</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar navigate to PuTTY and enter in your Host Name, port, and connection tyoe and click open<br/>
<img src="https://i.postimg.cc/GmbdH5XF/Screen-Shot-2023-03-03-at-12-42-34-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
type in the following commands to enter configuration mode  <br>
enable <br>
configure terminal <br>
<img src="https://i.postimg.cc/gJmv5dsw/Screen-Shot-2023-03-03-at-12-45-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
Enter the following commands to creat a new VLAN <br>
vlan 10 <br>
name ucertify <br>
exit <br>
interface range e0/2-3 <br>
switchport access vlan 10 <br>
end <br>
<img src="https://i.postimg.cc/LsnX8Wsy/Screen-Shot-2023-03-03-at-12-48-30-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
Enter the following commands to save the setting<br>
copy running-config startup-config <br>
show vlan <br>
<img src="https://i.postimg.cc/x8bMNCT4/Screen-Shot-2023-03-03-at-12-51-21-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />

 
