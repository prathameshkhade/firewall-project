# Pre-requisites

## Your understanding with the technologies
This project requires a foundational understanding of networking concepts. This includes:

*   **IP Addressing:** The unique identifier assigned to each device on a network.

*   **Subnetting:** Dividing a network into smaller logical segments.
*   **Routing:** The process of forwarding data packets between networks.
*   **Virtualization:** Creating virtual machines (VMs) that run on a single physical computer.

*   **Operating System Installation:** Familiarity with installing operating systems, both physically and virtually.

## Explanation of Concepts | Terminologies

*   **Virtualization Software:** Allows you to create and run multiple operating systems on a single physical computer. This enables simulating a network environment on your personal machine.

*   **ISO Files:** Disc image files containing the installation data for operating systems. These are used to install the chosen operating systems within your virtual machines.

*   **Guest Operating Systems:** The operating systems installed within the virtual machines. These will represent the different servers and workstations in your simulated network.

*   **Firewall:** Software or Hardware or combination of both which is used to manage and moniter the data packets according to some pre-defined rules. 


## Requirements

### Software Requirements
Download the following softwares

1.  **Virtualization Software:** For installing multiple operating systems on your system you required a virtualization software which will be installed on the host OS (your current OS). You can either download any one of the following as per your current OS.
    *   [Virtualbox](https://www.virtualbox.org/wiki/Downloads) or [VMware](https://www.vmware.com/info/workstation-player/evaluation) for Windows or Linux
    *   [QEMU](https://www.qemu.org/download/#macos) for MacOS
  
2. **Guest Operating Systems (VMs):** You required the ISO file of the OS for installing the OS virtually. Download any of the following OS as per your system compatibility
   *   [**PfSense Firewall:**](https://www.pfsense.org/download) (Open-Source, Free) - This firewall software will be installed within a VM and act as both a router and firewall for your simulated network.
   *    [**Ubuntu Server 24.04 LTS**](https://ubuntu.com/download/server): (Open-Source, Free) - A popular Linux server distribution. This project will configure FTP, SSH, and email servers and many more on this VM.
   *   [**Windows 7/10:**](https://www.microsoft.com/en-in/software-download/windows10) Obtain installation media for Windows. These VMs will simulate client machines.
   *   [**Arch Linux:**](https://archlinux.org/download) (Open-Source, Free) - Advanced Linux distribution for experienced users (optional).
   *   [**Metasploitable 2:**](https://sourceforge.net/projects/metasploitable/) (Open-Source, Free) - A test environment provides a secure place to perform penetration testing and security research. You can use this instrad of setting all the things. It consist of pre-installed services including HTTP, HTTPS, RDP, FTP, DNS, IMAP, etc.

### Hardware Requirements
This project is designed to run on a personal computer with the following minimum specifications:

*   **CPU:** Processor with at least 4 cores (more cores improve performance)
*   **RAM:** 8 GB or more (additional RAM allows for more complex virtual machines)
*   **Storage:** 20 GB or more (space for the host operating system, virtual machines, and project files)

Configuration of my HP Notebook is...
1.  **CPU:** Intel i3-5005U (4) @ 1.900GHz
2.  **GPU:** Intel HD Graphics 5500
3.  **GPU:** AMD ATI Radeon HD 8670A/8670M/8690M / R5 M330 / M430 / Radeon 520 Mobile
4.  **RAM:** 8 GB
5.  **Storage:** 256 GB SSD + 1 TB HDD
6.  **OS:** Kali GNU/Linux Rolling x86_64 24.3


## Conclusion
By gathering the necessary software and hardware, and familiarizing yourself with the listed concepts, you'll be well-prepared to embark on this firewall implementation project.

<div style='width:100%; display:flex; justify-content:space-between; algin-items:center' > 
    <button style='width:20%; height:30px; border-radius:20px; cursor:pointer' >Previous</button>
    <button style='width:20%; height:30px; border-radius:20px; cursor:pointer' >Next</button>
</div>