# Azure Network Security Groups (NSGs) and Traffic Analysis Between Azure Virtual Machines

> **Project Type:** Azure Networking Lab
> **Platform:** Microsoft Azure
> **Tools:** Azure Portal, Wireshark, PowerShell, Remote Desktop, Ubuntu Linux

---

# Project Overview

In this hands-on Azure networking lab, I deployed a Windows 10 Virtual Machine and an Ubuntu Linux Virtual Machine inside the same Azure Virtual Network to observe how network traffic flows between cloud resources.

Using Wireshark, I captured and analyzed multiple networking protocols while configuring Azure Network Security Groups (NSGs) to understand how Azure firewalls affect communication between virtual machines.

This project demonstrates practical cloud networking, troubleshooting, firewall administration, packet analysis, and virtual machine management skills commonly used by Help Desk, System Administrators, and Cloud Support Engineers.

---

# Architecture

```text
Azure Subscription
│
└── Resource Group
    │
    └── Virtual Network (VNet)
        │
        └── Subnet
            ├── Windows 10 Virtual Machine
            │
            └── Ubuntu Linux Virtual Machine
```

---

# Technologies Used

* Microsoft Azure
* Azure Virtual Machines
* Azure Resource Groups
* Azure Virtual Network (VNet)
* Azure Subnets
* Azure Network Security Groups (NSGs)
* Windows 10
* Ubuntu Linux
* Microsoft Remote Desktop
* Wireshark
* PowerShell
* SSH

---

# Skills Demonstrated

* Azure Administration
* Cloud Networking
* Virtual Machine Deployment
* Network Security Groups (NSGs)
* Network Troubleshooting
* Packet Analysis
* ICMP
* SSH
* DHCP
* DNS
* Remote Desktop Protocol (RDP)
* Firewall Configuration
* PowerShell

---

# Lab Activities

---

## 1. Azure Infrastructure

### Tasks Completed

* Created an Azure Resource Group
* Created a Virtual Network
* Created a Subnet
* Deployed a Windows 10 Virtual Machine
* Deployed an Ubuntu Linux Virtual Machine
* Verified both virtual machines were connected to the same Virtual Network

### Screenshots

Azure Resource Group

<img width="1488" height="737" alt="Resource Group" src="https://github.com/user-attachments/assets/62f56578-5c48-45d6-9297-2105e21539c0" />


Virtual Network

<img width="850" height="733" alt="Virtual Network" src="https://github.com/user-attachments/assets/ca930f96-5dd2-4087-91ad-4e53aac4cf02" />


Windows Virtual Machine

<img width="877" height="730" alt="Windows-VM" src="https://github.com/user-attachments/assets/c8a4eec3-d3a3-40fe-b6d3-03bfc4d862b2" />


Ubuntu Virtual Machine

<img width="988" height="742" alt="Linux-VM" src="https://github.com/user-attachments/assets/f7be37c0-6182-4627-94c8-5935fed82f75" />


---

## 2. ICMP Traffic Analysis

### Tasks Completed

* Installed Wireshark
* Started packet capture
* Filtered ICMP packets
* Retrieved the Ubuntu VM private IP address
* Successfully pinged the Ubuntu VM
* Observed Echo Requests and Echo Replies

### Screenshots

📷 Wireshark ICMP Filter

<img width="1510" height="931" alt="ICMP Filter" src="https://github.com/user-attachments/assets/b89b536a-79d4-49de-99be-14e27fb2831f" />


📷 Successful Ping

<img width="1509" height="907" alt="Successful Ping" src="https://github.com/user-attachments/assets/40eb0e5b-2954-4ee4-8b19-38f3f9269b3f" />


---

## 3. Azure Network Security Groups (Firewall)

### Tasks Completed

* Configured inbound NSG rules
* Blocked ICMP traffic
* Verified ping requests failed
* Re-enabled ICMP traffic
* Confirmed communication resumed

### Screenshots

📷 NSG Rule

<img width="582" height="740" alt="NSG Rule" src="https://github.com/user-attachments/assets/27dc8f80-1d50-4e8f-91d5-bc05ea4a84d9" />


📷 Failed Ping

<img width="1508" height="911" alt="Failed Ping" src="https://github.com/user-attachments/assets/62b73d01-0fb4-41c8-a7b7-5650d164261e" />


📷 Successful Ping After Rule Change

<img width="1512" height="909" alt="Screenshot 2026-07-05 at 6 49 27 AM" src="https://github.com/user-attachments/assets/d3c03a7f-4c87-474f-a6f4-9703898c54b1" />


---

## 4. SSH Traffic

### Tasks Completed

* Connected to the Ubuntu VM using SSH
* Executed Linux commands
* Observed encrypted SSH packets inside Wireshark

### Screenshots

📷 SSH Connection

<img width="1508" height="905" alt="SSH" src="https://github.com/user-attachments/assets/f595977b-d896-4c11-9aa4-036c918669f1" />


📷 Wireshark SSH Traffic

<img width="1512" height="982" alt="Screenshot 2026-07-05 at 9 14 33 AM" src="https://github.com/user-attachments/assets/b96cd150-eee1-4334-b0f7-c5f832040592" />


---

## 5. DHCP Traffic

### Tasks Completed

* Renewed the Windows VM IP Address
* Observed DHCP traffic generated during the renewal process

### Screenshots

📷 DHCP Packet Capture

<img width="1512" height="886" alt="Screenshot 2026-07-06 at 7 05 57 AM" src="https://github.com/user-attachments/assets/fff020d0-f6ff-4f69-a357-59fc6dcc0221" />


---

## 6. DNS Traffic

### Tasks Completed

* Used nslookup to resolve domain names
* Captured DNS queries and responses using Wireshark

### Screenshots

📷 DNS Query

<img width="1512" height="910" alt="Screenshot 2026-07-06 at 7 15 43 AM" src="https://github.com/user-attachments/assets/3f8b31c6-c853-4f19-9153-b2d174ce2845" />


---

## 7. Remote Desktop Protocol (RDP)

### Tasks Completed

* Filtered Wireshark for TCP Port 3389
* Observed continuous RDP traffic

### Screenshots

📷 RDP Traffic

<img width="1506" height="913" alt="Screenshot 2026-07-06 at 7 29 39 AM" src="https://github.com/user-attachments/assets/f6080245-e54e-439c-92d8-ac172b57bead" />



---

# Project Structure

```text
Network-Security-Groups-NSGs-and-Inspecting-Traffic-Between-Azure-Virtual-Machines
│
├── README.md
│
├── images
│   ├── resource-group.png
│   ├── virtual-network.png
│   ├── windows-vm.png
│   ├── ubuntu-vm.png
│   ├── icmp.png
│   ├── nsg-rule.png
│   ├── ssh.png
│   ├── dhcp.png
│   ├── dns.png
│   └── rdp.png
│
└── documentation
    └── Lab Notes.pdf
```

---

# Video Walkthrough

## Full Demonstration

🎥 YouTube Video:

PASTE YOUR YOUTUBE LINK HERE

During this walkthrough I demonstrate:

* Deploying Azure Virtual Machines
* Creating a Virtual Network
* Configuring Network Security Groups
* Capturing packets with Wireshark
* Testing ICMP connectivity
* Observing SSH traffic
* Observing DHCP traffic
* Observing DNS traffic
* Observing Remote Desktop traffic

---

# Conclusion

In this tutorial, we explore network traffic between Azure Virtual Machines using Wireshark, focusing on different protocols such as ICMP, SSH, DHCP, DNS, and RDP. We also experiment with Network Security Groups (NSGs) to control inbound and outbound traffic. This allows us to gain insight into how network traffic flows between virtual machines and how security rules can be used to restrict or permit specific types of traffic. This lab strengthened my understanding of Azure networking and cloud infrastructure by providing hands-on experience deploying virtual machines, configuring virtual networks, capturing network traffic, troubleshooting connectivity issues, and managing Azure Network Security Groups.

---

