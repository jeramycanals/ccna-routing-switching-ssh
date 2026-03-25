<p align="center">
  <img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/69de9c93-46c5-486d-b60c-6fc096085465" />
  <img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/a445aca4-18d7-4d4f-b479-59ea2d1882f5" />
</p>

# Routing, Switching, and Secure SSH Configuration in Packet Tracer

This project is a hands-on Cisco Packet Tracer lab walkthrough that demonstrates the configuration of a basic network consisting of a router, switch, and two end devices. The lab focuses on building a functional network from scratch by assigning IP addressing, configuring network devices, and verifying connectivity between hosts.

In Part 1, devices are physically connected and configured with static IP addresses, while the router and switch are set up with basic security features such as encrypted passwords, console access, and a management interface. Network connectivity is then tested using ping to ensure proper communication between different subnets.

Part 2 involves using Cisco IOS commands to retrieve and interpret device information, including hardware details, routing tables, and interface status. This reinforces an understanding of how routers and switches operate and how to verify configurations in a real-world environment.

In Part 3, secure remote access is implemented by configuring SSH on the router. This includes setting a domain name, generating RSA keys, creating user credentials, and restricting VTY access to SSH only. The configuration is then tested to confirm successful remote login.

Overall, this lab provides foundational networking skills, including device configuration, troubleshooting connectivity, interpreting IOS output, and implementing secure remote management. These are key competencies for networking roles and CCNA knowledge.

<p align="center">
  <img width="776" height="208" alt="image" src="https://github.com/user-attachments/assets/b8623b08-b047-4dfa-b7c2-7c2e87b8623d" />
</p>

## Network Topology

<p align="center">
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

## Environments and Technologies Used

- Cisco Packet Tracer
- Cisco IOS (Router and Switch CLI)
- IPv4 Addressing and Subnetting
- Static IP Configuration
- VLAN (SVI for switch management)
- SSH (Secure Remote Access)
- Network Troubleshooting (Ping, Tracert)
- Routing (Directly Connected Networks)

## Operating Systems Used

- Windows (PC-A and PC-B simulation)
- Cisco IOS (Router and Switch operating system)

## Lab Objectives

[Part 1: Configure Devices and Verify Connectivity](#part-1--configure-devices-and-verify-connectivity)
- Assign static IP information to the PC interfaces.
- Configure the router and switch.
- Verify network connectivity.

[Part 2: Display Device Information](#part-2--display-device-information)
- Retrieve hardware and software information from the network devices.
- Interpret the output from the routing table.
- Display interface information on the router.
- Display a summary list of the interfaces on the router and switch.

[Part 3: Secure Remote Access to the Router](#part-3--secure-remote-access-to-the-router)
- Set the IP domain name and generate secure keys.
- Create an SSH user and configure VTY lines for SSH-only access.
- Verify SSH Implementation.

## Part 1: Configure Devices and Verify Connectivity

In Part 1, we will set up the network topology and configure basic settings, such as the interface IP addresses, device access, and passwords. We will refer to the Addressing Table for device names and address information.

### Step 1: Connect the devices.

#### Connect the devices using Copper Straight-Through cables as listed below:

- Connect PCA F0 to S1 F0/1.
- Connect S1 G0/1 to R1 G0/0/1
- Connect R1 G0/0/0 to PCB F0.
<img width="604" height="297" alt="image" src="https://github.com/user-attachments/assets/91f7aac9-15d1-4d40-87ca-df790905db6b" />

### Step 2: Assign static IP information to the PC interfaces.

#### a. Configure the IP address, subnet mask, and default gateway settings on PC-A according to the Addressing Table.
<img width="753" height="215" alt="image" src="https://github.com/user-attachments/assets/6e7fa358-b315-4a82-935a-380b5ef36e8b" />

#### b. Configure the IP address, subnet mask, and default gateway settings on PC-B.
<img width="751" height="210" alt="image" src="https://github.com/user-attachments/assets/3f509be5-af71-488d-80a1-31ba1203c474" />

#### c. Ping PC-B from a command prompt window on PC-A.
<img width="766" height="268" alt="image" src="https://github.com/user-attachments/assets/aafe61c0-a2d8-418a-abba-5ed38a541214" />

#### Why were the pings not successful?

The pings were not successful because the network devices (router and switch) in between the PCs have not been configured yet.

### Step 3: Configure R1 (Router).

#### a. Console into the router and enable privileged EXEC mode. Use console cable and terminal on a PC.
<img width="1027" height="148" alt="image" src="https://github.com/user-attachments/assets/b5b8370c-1145-49ca-aab3-429372fcf268" />
<img width="256" height="486" alt="image" src="https://github.com/user-attachments/assets/25458597-b0c9-4809-b41c-180848c3e9a5" />

#### b. Enter configuration mode.

<img width="438" height="43" alt="image" src="https://github.com/user-attachments/assets/487ca9a5-0648-425a-a0f2-13235cceb831" />

#### c. Assign a device name to the router according to the Addressing Table.

<img width="216" height="29" alt="image" src="https://github.com/user-attachments/assets/e89808ae-a29d-413b-be60-804fbcc21318" />

#### d. Assign class as the privileged EXEC encrypted password.

<img width="253" height="26" alt="image" src="https://github.com/user-attachments/assets/9e5d94d8-b35e-4be5-99fb-9cdfe72a7245" />

#### e. Assign cisco as the console password and enable login.

<img width="224" height="64" alt="image" src="https://github.com/user-attachments/assets/8f9ec2e7-5ec0-40ac-b815-5c4d16cc227d" />

#### f. Encrypt the plaintext passwords.

<img width="273" height="27" alt="image" src="https://github.com/user-attachments/assets/2d3ab5c5-6ca9-46a8-96d0-7784f2b824a7" />

#### g. Create a banner that warns anyone accessing the device that unauthorized access is prohibited.

<img width="421" height="26" alt="image" src="https://github.com/user-attachments/assets/1d02ad2b-95b6-4f7e-8858-16a874b10f6c" />

#### h. Configure the IP addresses according to the Addressing Table and activate both Ethernet interfaces on the router.

<img width="628" height="275" alt="image" src="https://github.com/user-attachments/assets/85e693e6-627a-484e-ba40-1d8d40d886ed" />

#### i. Save the running configuration to the startup configuration file.

<img width="293" height="69" alt="image" src="https://github.com/user-attachments/assets/ea33a6b1-f1c5-4350-8554-2fec2d165f24" />

#### j. Ping PC-B from a command prompt window on PC-A again.

<img width="766" height="521" alt="image" src="https://github.com/user-attachments/assets/d7edc3d2-dd75-41c4-9f13-2dd3f99684ca" />

#### Were the pings successful this time? Why?

Yes, the pings were successful. In the first ping attempt, the first packet timed out, but the next three packets were received successfully. This happens because the device must first perform ARP (Address Resolution Protocol) to learn the MAC address of the destination or the default gateway. During this process, the first ping request may fail while the ARP table is being updated with the correct MAC address. As shown in the screenshot, the first ping resulted in 1 packet lost (25% loss). However, when the ping command was run again, all four packets were received successfully with 0% packet loss, confirming that the network connectivity between the devices is functioning correctly. Once the ARP information was stored in the device’s ARP cache, communication between the devices happened without any further issues.

### Step 4: Configure S1 (Switch).

#### a. Console into the switch and enable privileged EXEC mode.

<img width="1121" height="143" alt="image" src="https://github.com/user-attachments/assets/7a96def1-d3b3-44bf-baae-940f8ac285cf" />

<img width="249" height="497" alt="image" src="https://github.com/user-attachments/assets/8629e294-9eb6-4605-9275-1632802e7c64" />

#### b. Enter configuration mode.

<img width="450" height="42" alt="image" src="https://github.com/user-attachments/assets/b03ade85-e65e-4b26-8a68-3511bb0a8ba8" />

#### c. Assign a device name to the switch according to the Addressing Table.

<img width="198" height="25" alt="image" src="https://github.com/user-attachments/assets/c237d139-d2d4-42cd-9c2f-c0e44f69b8c2" />

#### d. Assign class as the privileged EXEC encrypted password.

<img width="230" height="28" alt="image" src="https://github.com/user-attachments/assets/cd0c5557-0eea-402e-9ee9-828598e57fc3" />

#### e. Assign cisco as the console password and enable login.

<img width="217" height="66" alt="image" src="https://github.com/user-attachments/assets/7a699354-0783-4fe4-a58a-4f5809a3a16d" />

#### f. Encrypt the plaintext passwords.

<img width="277" height="27" alt="image" src="https://github.com/user-attachments/assets/9d978308-39b5-40c2-a486-62227fa245d3" />

#### g. Create a banner that warns anyone accessing the device that unauthorized access is prohibited.

<img width="421" height="27" alt="step4g" src="https://github.com/user-attachments/assets/824fd37b-db26-4e15-bcf3-ce7fcaef6eed" />

#### h. Configure the IP address for the SVI for VLAN 1 according to the Addressing Table and activate the interface.

<img width="527" height="144" alt="image" src="https://github.com/user-attachments/assets/454e19de-4c7d-46c1-a533-40d53bcfc250" />

#### i. Configure the default gateway according to the Addressing Table.

<img width="295" height="27" alt="image" src="https://github.com/user-attachments/assets/566a7243-5315-4098-9057-d7b73577a5ad" />

#### j. Save the running configuration to the startup configuration file.

<img width="289" height="64" alt="image" src="https://github.com/user-attachments/assets/3545e4a0-697e-4bda-8b86-e9c81ed8f833" />

### Part 1 Summary

In this part of the lab, a basic network topology was set up and configured to establish communication between devices. The process began by physically connecting the devices using the correct interfaces: PC-A to the switch, the switch to the router, and the router to PC-B.

Static IP addresses, subnet masks, and default gateways were then assigned to both PCs. Initial connectivity tests (ping) between PC-A and PC-B were unsuccessful because the router had not yet been configured to route traffic between the two networks.

Next, the router (R1) was configured with a hostname, secure passwords, encrypted credentials, and a login banner. IP addresses were assigned to both router interfaces and activated, enabling routing between networks. After this configuration, connectivity between the PCs was successfully established.

Finally, the switch (S1) was configured with basic security settings, including passwords and encryption, along with a management IP address using VLAN 1 (SVI). A default gateway was also configured to allow remote management of the switch from other networks. The configuration was saved to ensure persistence after reboot.

## Part 2: Display Device Information

In Part 2, we will use Cisco IOS commands to retrieve and analyze information from the router and switch. This includes examining hardware and software details, viewing the routing table, and checking interface status. These steps help verify device configurations and build a deeper understanding of how the network operates and reports its current state.

### Step 1: Retrieve hardware and software information from the network devices.

#### a. Use the show version command to answer the following questions about the router.

#### R1# show version

<img width="679" height="351" alt="part_2_step_1a" src="https://github.com/user-attachments/assets/bb52b934-ea39-4d69-b320-2afac335a2ce" />

#### What is the name of the IOS image that the router is running?

The system image file is "bootflash:/isr4300-universalk9.03.16.05.S.155-3.S5-ext.SPA.bin".

#### b. Use the show version command to answer the following questions about the switch.

#### S1# show version

<img width="680" height="523" alt="image" src="https://github.com/user-attachments/assets/a143b1fd-1588-44c5-a5f4-b1445ece9bf8" />

#### What is the IOS software image and version running on the switch?

The IOS software image and version running on the switch is Cisco IOS Software, C2960 Software (C2960-LANBASE-M), Version 12.2(25)FX, RELEASE SOFTWARE (fc1).

#### What is the model number of the switch?

The model number of the switch is WS-C2960-24TT.

### Step 2: Display the routing table on the router.

#### Use the show ip route command on the router to answer the following questions.

#### R1# show ip route

<img width="563" height="253" alt="image" src="https://github.com/user-attachments/assets/7ba8764a-746e-434b-9c88-460d61e83de2" />

#### What code is used in the routing table to indicate a directly connected network?

#### How many route entries are coded with a C code in the routing table?

#### What interface types are associated to the C coded routes?

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### Step 3: Display interface information on the router.

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### Step 4: Display a summary list of the interfaces on the router and switch.

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### Part 2 Summary

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## Part 3: Secure Remote Access to the Router

### Step 1 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### Part 3 Summary

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## Conclusion

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## Thank you for checking out my project!

If you found it helpful or interesting, subscribe to my YouTube channel and 🔗connect with me on LinkedIn by clicking below:

[<img align="left" alt="Jeramy | YouTube" width="22px" src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/youtube.svg" />][youtube]
[<img align="left" alt="Jeramy | LinkedIn" width="22px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" />][linkedin]

[youtube]: https://youtube.com/@jeramycanals
[linkedin]: https://linkedin.com/in/jeramycanals
