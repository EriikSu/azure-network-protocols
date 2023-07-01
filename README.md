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

- Windows 10 (22H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1: Create a Resource Group and 2 virtual machines (VM) in Microsoft Azure. One will be with Windows 10 and the other with Ubuntu. 
- Step 2: Will be using RDP (remote desktop) to connect to our Windows 10 VM and Install Wireshark.
- Step 3: Open WireShark and filter for ICMP traffic Only. Retrieve the private IP address of Ubuntu VM and attempt to ping it from within Windows 10 VM and     observe ping requests and replies within Wireshark.
- Step 4: Initiate a non-stop ping from Windows 10 VM to Ubuntu VM. Open the Network Security Group in Azure for the Ubuntu VM and disabling incoming (inbound) ICMP traffic. Back in Windows 10 VM, observe the ICMP traffic in WireShark and the command line in Ping Activity (It should block incoming traffic).
- Step 5: From within Windows 10 VM, "SSH into" the Ubuntu VM (via it's private IP address), and observe traffic then exit SSH.
- Step 6: In Windows 10 VM, attempt to issue a new IP address from the command line (ipconfig /renew) and observe DHCP traffic.
- Step 7: In Windows 10 VM, either powershell or command line we will use nslookup command to see what www.google.com is and observe DNS traffic in WireShark.
- Step 8: Observe ongoing RDP traffic in Wireshark

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
