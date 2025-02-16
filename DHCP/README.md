# DHCP Configuration

## Objective
Configure a DHCP server on a router to automatically assign IP addresses to PCs.

## Steps
1. Configured the router as a DHCP server:
   - Created a DHCP pool: `ip dhcp pool LAN`
   - Specified the network: `network 192.168.1.0 255.255.255.0`
   - Set the default gateway: `default-router 192.168.1.254`
   - Excluded reserved IPs: `ip dhcp excluded-address 192.168.1.1 192.168.1.10`
2. Set the PCs to obtain IP addresses automatically (DHCP).
3. Verified IP assignment using the `ipconfig` command.

## Screenshots
![image](https://github.com/user-attachments/assets/58ecbcf3-49e3-4b92-9080-bf9d261adc90)
![image](https://github.com/user-attachments/assets/20f42dc4-ecbd-41c6-bd9a-643fe1fc66e8)



## Outcome
Successfully assigned IP addresses to PCs using DHCP.
