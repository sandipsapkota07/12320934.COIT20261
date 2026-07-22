# COIT20261 Portfolio – Week 01

**Student Name:** Sandip Sapkota  
**Student ID:** 12320934
**Unit:** COIT20261  
**Week:** 01  
**Date:** 19 July 2026

## Objective

The objective of this week's tutorial was to become familiar with the unit requirements, set up the required software, create the GitHub repository, and gain introductory experience with GNS3 by creating a simple network project and configuring a Linux host with a static IP address.

# Section A
## Tasks Completed

- Reviewed the COIT20261 Unit Profile and assessment requirements.
- Confirmed installation of:
  - VirtualBox
  - GNS3
- Created a private GitHub repository for the unit.
- Created the Week 01 portfolio file using Markdown.


# Section B – GNS3 Introduction
## Project Information

**Project Name**

```
GNS3-Intro-12320934
```

### Activities Completed

- Created a new GNS3 project.
- Added one Linux Host node.
- Added project annotations including:
  - Student Name
  - Student ID
  - Date
  - Project Title
- Selected and configured a static IP address.
- Edited the `/etc/network/interfaces` file before starting the node.
- Started the Linux host.
- Opened the Web Console.
- Verified the configured IP address using Linux commands.

# Network Configuration

| Item | Value |
|------|-------|
| Host | Linux Host |
| Interface | eth0 |
| IP Address | 10.10.4.0 |
| Netmask | 255.255.255.0 |

Example configuration used:

```text
auto eth0
iface eth0 inet static
    address 10.10.1.1
    netmask 255.255.255.0
    up sysctl net.ipv4.ip_forward=0
```
# Commands Used
### Show IP Address

```bash
ip a
```

# Evidence

- ![Computer Info](images/nsa-1.png)
- ![Computer Info](images/nsa-2.png)
- ![Computer Info](images/nsa-3.png)



# Testing Results

| Test | Result |
|------|--------|
| Linux Host Started Successfully |  Pass |
| Static IP Configured |  Pass |
| IP Address Verified |  Pass |
| GNS3 Project Saved Successfully |  Pass |

# Challenges

- Initially understanding how to edit the `/etc/network/interfaces` configuration file.
- Learning the difference between dynamic (DHCP) and static IP addressing.
- Becoming familiar with the GNS3 interface and Linux terminal.

# Reflection

This week's practical introduced me to the basic features of GNS3 and Linux networking. I learned how to create a network project, add a Linux host, configure a static IP address, and verify the configuration using Linux commands. I also gained experience using Markdown for documenting practical work in GitHub.

Although the activities were relatively simple, they helped me understand the importance of proper network configuration and documentation. I became more confident using the Linux terminal and navigating the GNS3 environment.

For future weeks, I plan to improve my knowledge of Linux networking commands, GitHub documentation, and GNS3 network simulations.

# Learning Outcomes

After completing Week 01, I can:

- Create a GNS3 project.
- Add and configure a Linux Host.
- Configure a static IP address.
- Use Linux commands to verify network configuration.
- Document practical work using Markdown.
- Organise portfolio evidence in GitHub.
