<p align="center">
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/bab0e33b-b94d-4ed9-be6e-a038d82889c7" width="500"/>
</p>

<h1>Network Activity Monitoring with Wireshark - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the Network Activity Monitoring with Wireshark lab. 
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Wireshark
- Remote Desktop
- Client 1 VM
- Client 2 VM

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> 
- Ubuntu 20.04</b> 

<h2>Create the Virtual Machines</h2>

<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/745f66ae-390d-4e57-969b-c58a8018bd0f" width="400"/>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/2f562165-5679-411f-8104-0fce80f2e094" width="400"/>
</p>
<p>
Make sure both VMs are created on the same vnet and resource group.
Log into Client 1 (4.227.147.96) through RDP.
</p>
<p>
Note the private IP address for the Windows client as: 10.0.0.4 and the private IP address for Linux as: 10.0.0.5.
</p>
<br />

<h2>Observe ICMP Traffic</h2>
<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/0242afc0-bd2d-4f6c-ab7a-6bcd3000edcf" width="800"/>
</p>
<p>
From the Windows VM, Ping the Linux VM and ping www.google.com and observe the traffic in wireshark.
</p>
<br />

<h2>Observe SSH Traffic</h2>
<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/7b510fe8-6bd4-4078-99b0-72f3f7f232e4" width="800"/>
<img src="" width="400"/>
</p>
<p>
From the Windows VM, SSH into the Linux VM with ssh Kaid@10.0.0.5. Type in linux commands in the command line and observe the traffic.
</p>
<br />

<h2>Observe DHCP Traffic</h2>

<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/73e43095-519a-4818-90a2-e2e7ccc56091" width="800"/>
</p>
<p>
From the Windows VM, on the command line type ipconfig /renew and oberserve the traffic.
</p>
<br />

<h2>Observe DNS Traffic</h2>

<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/8c708694-ac40-46a3-9b53-254c827ec1e1" width="800"/>
</p>
<p>
From the Windows VM, use nslookup for any website and observe the traffic in wireshark.
</p>
<br />

<h2>Observe RDP Traffic</h2>
<p>
<img src="https://github.com/ronnydiggs/azure-network-protocols/assets/64152064/f349624a-a5fe-41b7-ac1a-a4a647b71682" width="800"/>
</p>
<p>
Filter for RDP. Notice the number of packets is in the upper 90%.
</p>
<br />


