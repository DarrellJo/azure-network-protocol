<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we will guide you through the process of observing network traffic between two Azure Virtual Machines using the open-source tool Wireshark.

<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://youtu.be/rh6UmkmTUHY)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, DHCP, DNS, RDP, ICMP)
- [Wireshark](https://www.wireshark.org/download.html) (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- ICMP (Internet Control Message Protocol; No Port #)
- SSH (Secure Shell; TCP Port 22)
- DHCP (Dynamic Host Configuratiion Protocol; UDP Port 67 & 68)
- DNS (Domain Name Server; TCP Port 53)
- RDP (Remote Desktop Protocol; TCP Port 3389)


<h2>Actions and Observations</h2>
To get started, follow these steps:

1. Create a resource group that includes two virtual machines: one with Windows 10 and the other with Ubuntu (Linux).
2. Remote into both virtual machines to access their respective desktop environments.
3. Download Wireshark onto your Windows 10 machine.
4. Proceed with the following steps to observe network traffic between the two virtual machines.<br />

<h3>Internet Control Message Protocol (IMCP) </h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
ICMP, short for Internet Control Message Protocol, is a network protocol that functions at the network layer of the Internet Protocol Suite. ICMP is widely recognized as the "ping" protocol, as it enables network connectivity testing and facilitates the measurement of round-trip times between two devices. This is accomplished through the exchange of Echo Request and Echo Reply messages.
</p>
<br />

<h3> Secure Shell (SSH) </h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
SSH, which stands for Secure Shell, is a network protocol specifically designed for secure remote login, command execution, and data communication between two networked devices. It establishes a secure channel over potentially insecure networks, like the internet, by encrypting all data transmitted between the client and server.

In our lab, we utilize SSH to securely access and manage our Ubuntu/Linux virtual machine (VM). By leveraging SSH, we can establish a protected connection to the VM, ensuring that our remote login sessions and data transfers are encrypted and safeguarded against unauthorized access. SSH enables us to remotely interact with the VM's command-line interface and execute commands securely, providing a reliable and secure method for managing our virtual environment.
</p>
<br />

<h3> Dynamic Host Configuration Protocol (DHCP) </h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
DHCP, or Dynamic Host Configuration Protocol, is a network protocol used to automatically assign IP addresses and other network configuration parameters to devices on a network. It simplifies the process of network setup and management by dynamically allocating IP addresses rather than requiring manual configuration for each device.
</p>
<br />

<h3> Domain Name Server (DNS) </h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
DNS, which stands for Domain Name System, is a fundamental protocol used to translate domain names into IP addresses on the internet. It serves as a distributed database that stores and retrieves information associated with domain names.

Here's an overview of DNS:

DNS resolves domain names, such as www.disney.com, into their corresponding IP addresses, such as 192.195.66. This translation is necessary for devices to locate and communicate with websites, services, and other resources on the internet.

</p>
<br />

<h3> Remote Desktop Protocol </h3>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Remote Desktop Protocol (RDP) is a network protocol developed by Microsoft that facilitates remote access and control of computers or virtual machines. With RDP, users can establish a remote connection to a host computer and interact with its desktop environment as if they were sitting in front of it.

By leveraging RDP, users can perform various tasks and operations on the remote system, including accessing files, running applications, managing settings, and performing administrative tasks. RDP transmits the graphical user interface (GUI) of the remote desktop to the client device, allowing users to view and control the remote system's desktop environment in real-time.
</p>
<br />

