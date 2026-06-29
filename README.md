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

📷 Azure Resource Group

(Add Screenshot Here)

📷 Virtual Network

(Add Screenshot Here)

📷 Windows Virtual Machine

(Add Screenshot Here)

📷 Ubuntu Virtual Machine

(Add Screenshot Here)

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

(Add Screenshot Here)

📷 Successful Ping

(Add Screenshot Here)

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

(Add Screenshot Here)

📷 Failed Ping

(Add Screenshot Here)

📷 Successful Ping After Rule Change

(Add Screenshot Here)

---

## 4. SSH Traffic

### Tasks Completed

* Connected to the Ubuntu VM using SSH
* Executed Linux commands
* Observed encrypted SSH packets inside Wireshark

### Screenshots

📷 SSH Connection

(Add Screenshot Here)

📷 Wireshark SSH Traffic

(Add Screenshot Here)

---

## 5. DHCP Traffic

### Tasks Completed

* Renewed the Windows VM IP Address
* Observed DHCP traffic generated during the renewal process

### Screenshots

📷 DHCP Packet Capture

(Add Screenshot Here)

---

## 6. DNS Traffic

### Tasks Completed

* Used nslookup to resolve domain names
* Captured DNS queries and responses using Wireshark

### Screenshots

📷 DNS Query

(Add Screenshot Here)

---

## 7. Remote Desktop Protocol (RDP)

### Tasks Completed

* Filtered Wireshark for TCP Port 3389
* Observed continuous RDP traffic

### Screenshots

📷 RDP Traffic

(Add Screenshot Here)

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

# Key Takeaways

This lab strengthened my understanding of Azure networking and cloud infrastructure by providing hands-on experience deploying virtual machines, configuring virtual networks, capturing network traffic, troubleshooting connectivity issues, and managing Azure Network Security Groups.

Working through this project reinforced how common networking protocols operate in a cloud environment and how Azure security controls influence communication between virtual machines.

---

