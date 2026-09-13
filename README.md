# 🔐 Cybersecurity Lab Environment Setup

Building an isolated virtual lab for penetration testing and ethical hacking practice

# 📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

# 🎯 Objectives

The main objectives of this project are to:

• Install and configure VirtualBox.
• Install/import Kali Linux as a virtual machine.
• Create a private NAT Network for the cybersecurity lab.
• Configure network connectivity for Kali Linux.
• Assign a consistent IP address to the Kali VM.
• Verify network connectivity and DNS resolution.
• Take a clean VM snapshot for recovery.
• Document the complete setup process.
• Prepare the environment for future cybersecurity projects.

# 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

• Network reconnaissance
• Port scanning
• Vulnerability assessment
• Packet analysis
• Web security testing
• Exploitation practice
• Security-tool experimentation

⚠️ Important: This laboratory must only be used for systems that you own or have explicit permission to test. Do not use the lab or its tools to attack unauthorized systems.

# 🏗️ Lab Architecture

![Lab Architecture](./images/lab-diagram.png)

Additional target machines can be added to the same virtual network in future projects.


## ⚙️ Lab Configuration

| 🧩 Component | ⚙️ Configuration |
| :--- | :--- |
| 💻 **Host OS** | Windows 10 |
| 🧠 **Host RAM** | 8 GB |
| ⚡ **Processor** | Intel Core i7 |
| 🧰 **Hypervisor** | VirtualBox 7.2 |
| 🐉 **Security OS** | Kali Linux 2026.2 |
| 🧠 **Kali RAM** | 2048 MB (2 GB) |
| 📦 **Target VM 1** | Metasploitable 2 |
| 🛡️ **Target VM 2** | Windows Server 2019 |
| 🌐 **Network Mode** | NAT Network (Isolated) |

# 🪜 Lab Setup Procedure

# Step 1. Install 7-Zip

7-Zip was installed to extract the Kali Linux virtual-machine package, which may be distributed as a .7z archive.

Tool: 7-Zip

# Step 2. Install VirtualBox

VirtualBox was installed as the hypervisor.

# Step 3. Create the NAT Network

A dedicated NAT Network was created in VirtualBox.

Configuration: Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Enabled IPv6: Disabled

