# Week 03 – Enterprise Server Deployment and Operating System Installation

## Project Overview

This project focuses on deploying and configuring an Ubuntu Server virtual machine using enterprise-oriented system administration practices. The activity covers operating system installation, virtual machine configuration, basic server configuration, system verification, and documentation of the boot process.

The project also examines the differences between BIOS and UEFI firmware and explains how a computer proceeds from power-on to operating system startup.

---

## Learning Objectives

By completing this project, I was able to:

* Deploy Ubuntu Server inside a virtual machine.
* Configure appropriate virtual machine resources.
* Perform a clean Ubuntu Server installation.
* Configure basic server settings.
* Verify that the installed operating system is working correctly.
* Understand the differences between BIOS and UEFI.
* Explain the computer boot process.
* Practice documenting system administration procedures.
* Organize technical documentation using GitHub.

---

## Virtual Machine Specifications

| Component               | Specification                           |
| ----------------------- | --------------------------------------- |
| Virtualization Platform | VirtualBox                              |
| Operating System        | Ubuntu Server                           |
| Architecture            | 64-bit                                  |
| CPU                     | 2 Virtual CPUs                          |
| RAM                     | 4 GB                                    |
| Virtual Disk            | 25 GB                                   |
| Network                 | NAT                                     |
| Installation Media      | Ubuntu Server ISO                       |
| Firmware                | UEFI/BIOS depending on VM configuration |

> **Note:** The virtual disk used for this project is 25 GB.

---

## Installation Summary

The Ubuntu Server virtual machine was created using Oracle VirtualBox. The virtual machine was configured with the required CPU, memory, storage, and network settings before starting the installation.

The Ubuntu Server ISO image was mounted as the virtual optical disk. During installation, the following major steps were completed:

1. Started the Ubuntu Server virtual machine.
2. Selected the appropriate installation language.
3. Configured keyboard settings.
4. Configured network connectivity.
5. Selected the default Ubuntu Server installation.
6. Configured the 25 GB virtual disk.
7. Created the server user account.
8. Configured the server name.
9. Installed the OpenSSH Server option when required.
10. Completed the Ubuntu Server installation.
11. Rebooted the virtual machine.
12. Removed/ejected the installation ISO after installation.
13. Logged into the newly installed Ubuntu Server system.

---

## Configuration Summary

After installation, the Ubuntu Server system was checked and configured to ensure that it was ready for basic server administration.

The following configuration tasks were performed:

* Verified the hostname.
* Verified the assigned IP address.
* Checked network connectivity.
* Updated the package repository information.
* Updated installed packages.
* Verified available disk space.
* Verified memory allocation.
* Verified CPU information.
* Checked the operating system version.
* Confirmed that the server could communicate through the network.

Example commands used for verification and administration:

```bash
hostnamectl
```

```bash
ip addr
```

```bash
ping -c 4 google.com
```

```bash
lsb_release -a
```

```bash
df -h
```

```bash
free -h
```

```bash
lscpu
```

---

## Verification Results

The Ubuntu Server installation was successfully verified after the system rebooted.

| Verification                     | Result |
| -------------------------------- | ------ |
| Ubuntu Server boots successfully | Passed |
| User can log in                  | Passed |
| Hostname is configured           | Passed |
| Network interface detected       | Passed |
| IP address assigned              | Passed |
| Internet connectivity            | Passed |
| Disk detected                    | Passed |
| RAM detected                     | Passed |
| CPU detected                     | Passed |
| Ubuntu version verified          | Passed |

The commands listed in the Configuration Summary were used to confirm that the virtual machine was functioning correctly.

---

## BIOS vs UEFI Highlights

BIOS and UEFI are firmware interfaces responsible for initializing hardware and starting the operating system boot process.

| BIOS                                 | UEFI                                 |
| ------------------------------------ | ------------------------------------ |
| Older firmware standard              | Modern firmware standard             |
| Uses traditional boot process        | Uses a more advanced boot manager    |
| Commonly works with MBR              | Commonly works with GPT              |
| More limited interface               | Supports graphical interfaces        |
| Limited modern hardware features     | Supports newer hardware and features |
| Generally slower startup             | Generally faster startup             |
| Limited boot-management capabilities | Supports Secure Boot                 |

### Key Difference

BIOS is the traditional firmware interface used by older computers, while UEFI is its modern replacement. UEFI provides improved boot management, support for GPT partitions, Secure Boot, and compatibility with modern hardware.

---

## Embedded Boot Process Flowchart

The boot process can be summarized as:

```text
+------------------+
|   Power On       |
+--------+---------+
         |
         v
+------------------+
| Firmware Starts  |
| BIOS / UEFI      |
+--------+---------+
         |
         v
+------------------+
| Hardware Check   |
| POST / Hardware  |
| Initialization   |
+--------+---------+
         |
         v
+------------------+
| Find Boot Device |
+--------+---------+
         |
         v
+------------------+
| Bootloader       |
| GRUB             |
+--------+---------+
         |
         v
+------------------+
| Linux Kernel     |
| Loads            |
+--------+---------+
         |
         v
+------------------+
| systemd          |
| Initialization   |
+--------+---------+
         |
         v
+------------------+
| Ubuntu Server    |
| Login Prompt     |
+------------------+
```

---

## Challenges Encountered

Several challenges were encountered while setting up the virtual machine. One challenge was configuring the virtual machine storage correctly because the available virtual disk size was limited to 25 GB. Another challenge was ensuring that the Ubuntu Server ISO was properly mounted before starting the installation.

Network configuration was also checked carefully because the server needed network connectivity for package updates and verification. Understanding the difference between the virtual machine's hardware settings and the actual computer's hardware was another important part of the activity.

These challenges were resolved by checking the VirtualBox settings, verifying the ISO configuration, and using Linux commands to inspect the system after installation.

---

## Reflection

This activity helped me understand the practical process involved in deploying an operating system for server administration. Before completing the laboratory, I had a basic understanding of virtual machines and operating systems, but the installation process allowed me to see how the different components work together in an actual server environment.

One of the most important things I learned was how to properly configure a virtual machine before installing an operating system. CPU, RAM, storage, networking, and installation media all need to be configured correctly because an incorrect setting can prevent the operating system from installing or functioning properly. I also learned that even with limited resources, a virtual machine can be used to create a working server environment for learning and testing.

The Ubuntu Server installation also gave me experience with a Linux-based server operating system. Unlike a typical desktop operating system, Ubuntu Server focuses more on command-line administration and system management. Using commands such as `ip addr`, `hostnamectl`, `df -h`, `free -h`, and `lscpu` helped me understand how administrators inspect and verify a server.

Another important lesson was understanding the boot process. I learned that the computer does not immediately load the operating system after being powered on. The firmware first initializes the hardware, identifies a bootable device, and then transfers control to the bootloader. The bootloader loads the Linux kernel, after which system services are initialized until the system reaches the login prompt.

Learning about BIOS and UEFI also helped me understand how modern computers start their operating systems. UEFI provides more modern features such as GPT support and Secure Boot, while BIOS represents the older firmware standard.

Overall, this project improved my confidence in working with virtual machines and Linux servers. It also taught me the importance of documenting every configuration and verification step. These skills are useful for future system administration, networking, cybersecurity, and server deployment activities.

---

## References

https://ubuntu.com/download/serverhttps://ubuntu.com/download/serverv
https://www.microsoft.com/en-us/software-download/windows11
https://www.virtualbox.org/https://www.virtualbox.org/