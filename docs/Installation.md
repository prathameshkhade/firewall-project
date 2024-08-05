# Installation

Now I'm going to install the PfSense Firewall along with other client OS on Virtual Box.

## Installing pfSense on VirtualBox: A Step-by-Step Guide

### Step 1: Create a New Virtual Machine
1. **Open VirtualBox:** Launch the VirtualBox application on your system.
2. **Create a New Virtual Machine:** Click on the "New" button to start the virtual machine creation wizard.
3. **Name and Type:** Give a name to your virtual machine (e.g., "pfSense") and select "BSD" as the type and "FreeBSD (64-bit)" as the version.
4. **Memory Allocation:** Allocate at least 1GB of RAM for the virtual machine.
5. **Hard Disk Creation:** Choose "Create a virtual hard disk now" and select "VDI" as the hard disk file type.
6. **Storage Allocation:** Select "Dynamically allocated" for storage and specify the desired size (e.g., 20GB).
7. **Finish:** Click on the "Create" button to complete the virtual machine creation.

[Image of VirtualBox new virtual machine wizard]

### Step 2: Configure Virtual Machine Settings
1. **Access Settings:** Select the newly created virtual machine and click on the "Settings" button.
2. **System:**
   * Processor: Allocate at least 2 cores.
   * Chipset: Select "ICH9"
   * Enable PAE/NX
   * Enable IO APIC
3. **Network:**
   * Create two network adapters:
     * Adapter 1: Attach to "Host-only Adapter" for the LAN interface.
     * Adapter 2: Attach to "NAT" for the WAN interface.
4. **Storage:**
   * Select the "Empty" CD/DVD drive and click on the disk icon.
   * Choose the pfSense ISO image file you downloaded.
5. **Finish:** Click on "OK" to save the settings.

[Image of VirtualBox virtual machine settings]

### Step 3: Install pfSense
1. **Start the Virtual Machine:** Start the newly created virtual machine.
2. **Boot from ISO:** The virtual machine should boot from the pfSense installation media. Press any key when prompted.
3. **Installation Wizard:** Follow the on-screen instructions to install pfSense. The default options are usually sufficient.
4. **Interface Configuration:** Configure the network interfaces (WAN and LAN) during the installation process.
5. **Password:** Set a strong password for the administrator account.

[Image of pfSense installation wizard]

### Step 4: Initial Configuration
1. **Access pfSense Web Interface:** Once the installation is complete, you can access the pfSense web interface by opening a web browser on your host machine and entering the IP address of the pfSense virtual machine (usually 192.168.1.1).
2. **Login:** Use the administrator username and password you set during installation.
3. **System Setup:** Configure basic system settings like hostname, domain name, time zone, etc.
4. **Interface Configuration:** Assign IP addresses to the WAN and LAN interfaces.
5. **Firewall Rules:** Create basic firewall rules to allow necessary traffic.

[Image of pfSense web interface login]

### Additional Steps
* **DHCP Server:** Configure the LAN interface as a DHCP server to automatically assign IP addresses to connected devices.
* **DNS Server:** Configure a DNS server if required.
* **VPN:** Set up VPN services if needed.
* **Advanced Configuration:** Explore additional features like load balancing, failover, and more.

**Note:** This is a basic guide. For more advanced configurations and troubleshooting, refer to the official pfSense documentation.

By following these steps, you should have a pfSense firewall running in a virtual machine on your system. Remember to adjust the settings based on your specific network requirements.
 
**Would you like to proceed to the next step, which is configuring the firewall rules?**
