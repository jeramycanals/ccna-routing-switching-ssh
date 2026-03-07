<p align="center">
  <img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/69de9c93-46c5-486d-b60c-6fc096085465" />
  <img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/a445aca4-18d7-4d4f-b479-59ea2d1882f5" />
</p>

# Routing, Switching, and Secure SSH Configuration in Packet Tracer

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

<p align="center">
  <img width="776" height="208" alt="image" src="https://github.com/user-attachments/assets/b8623b08-b047-4dfa-b7c2-7c2e87b8623d" />
</p>

## Network Topology

<p align="center">
  <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

## Environments and Technologies Used

- lorem
- lorem
- lorem

## Operating Systems Used

- Cisco IOS (Internetwork Operating System)

## Lab Sections (High-Level Overview)

[Part 1 – Configure Devices and Verify Connectivity](#part-1--configure-devices-and-verify-connectivity)
- Assign static IP information to the PC interfaces.
- Configure the router and switch.
- Verify network connectivity.

[Part 2 – Display Device Information](#part-2--display-device-information)
- Retrieve hardware and software information from the network devices.
- Interpret the output from the routing table.
- Display interface information on the router.
- Display a summary list of the interfaces on the router and switch.

[Part 3 – Secure Remote Access to the Router](#part-3--secure-remote-access-to-the-router)
- Set the IP domain name and generate secure keys.
- Create an SSH user and configure VTY lines for SSH-only access.
- Verify SSH Implementation.

## Part 1 – Configure Devices and Verify Connectivity

In Part 1, we will set up the network topology and configure basic settings, such as the interface IP addresses, device access, and passwords. We will refer to the Addressing Table for device names and address information.

### Step 1: Connect the devices.

Connect the devices using Copper Straight-Through cables as listed below:

- Connect PCA F0 to S1 F0/1.
- Connect S1 G0/1 to R1 G0/0/1
- Connect R1 G0/0/0 to PCB F0.
<img width="604" height="297" alt="image" src="https://github.com/user-attachments/assets/91f7aac9-15d1-4d40-87ca-df790905db6b" />

### Step 2: Assign static IP information to the PC interfaces.

a.     Configure the IP address, subnet mask, and default gateway settings on PC-A according to the Addressing Table.
<img width="753" height="215" alt="image" src="https://github.com/user-attachments/assets/6e7fa358-b315-4a82-935a-380b5ef36e8b" />

b.     Configure the IP address, subnet mask, and default gateway settings on PC-B.
<img width="751" height="210" alt="image" src="https://github.com/user-attachments/assets/3f509be5-af71-488d-80a1-31ba1203c474" />

c.     Ping PC-B from a command prompt window on PC-A.
<img width="766" height="268" alt="image" src="https://github.com/user-attachments/assets/aafe61c0-a2d8-418a-abba-5ed38a541214" />

Why were the pings not successful?

The pings were not successful because the network devices (router and switch) in between the PCs have not been configured yet.

### Step 3: Configure R1 (Router).

a.     Console into the router and enable privileged EXEC mode. Use console cable and terminal on a PC.
<img width="1027" height="148" alt="image" src="https://github.com/user-attachments/assets/b5b8370c-1145-49ca-aab3-429372fcf268" />
<img width="256" height="486" alt="image" src="https://github.com/user-attachments/assets/25458597-b0c9-4809-b41c-180848c3e9a5" />

b.     Enter configuration mode.

<img width="438" height="43" alt="image" src="https://github.com/user-attachments/assets/487ca9a5-0648-425a-a0f2-13235cceb831" />

c.     Assign a device name to the router according to the Addressing Table.

<img width="216" height="29" alt="image" src="https://github.com/user-attachments/assets/e89808ae-a29d-413b-be60-804fbcc21318" />

d.     Assign class as the privileged EXEC encrypted password.

<img width="253" height="26" alt="image" src="https://github.com/user-attachments/assets/9e5d94d8-b35e-4be5-99fb-9cdfe72a7245" />

e.     Assign cisco as the console password and enable login.

<img width="224" height="64" alt="image" src="https://github.com/user-attachments/assets/8f9ec2e7-5ec0-40ac-b815-5c4d16cc227d" />

f.      Encrypt the plaintext passwords.

<img width="273" height="27" alt="image" src="https://github.com/user-attachments/assets/2d3ab5c5-6ca9-46a8-96d0-7784f2b824a7" />

g.     Create a banner that warns anyone accessing the device that unauthorized access is prohibited.

<img width="411" height="95" alt="image" src="https://github.com/user-attachments/assets/0efc36b4-9901-4491-a651-1822a9d4e48e" />

h.     Configure the IP addresses according to the Addressing Table and activate both Ethernet interfaces on the router.

i.      Save the running configuration to the startup configuration file.

Were the pings successful? Why?

### Part 1 Summary

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## Part 2 – Display Device Information

### Step 2 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### Part 2 Summary

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

## Part 3 – Secure Remote Access to the Router

### Step 3 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.

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
