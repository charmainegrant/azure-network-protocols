<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a Resource Group and Windows 10 VM.  
- Allow it to create a Vnet and Subnet.
- Create a Ubuntu (Linux) VM and choose the same  Resource Group and Vnet.  
- Access the Windows 10 VM via Remote Desktop
- Observe communication between VM's using various Network Protocols and commands.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/UpMZCUy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Command Prompt. Ping the private IP address of the Linux VM. Observe the ICMP traffic in WireShark
</p>
<br />

<p>
<img src="https://i.imgur.com/isKiVSx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Filter DHCP traffic only. Type ipconfig/renew in the command prompt to request a new IP address from your VM. Observe the traffic in WireShark and the commmand prompt.
</p>
<br />
