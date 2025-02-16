# Inter-VLAN Routing

## Objective
Configure a router to enable communication between two VLANs.

## Steps
1. Created two VLANs on the switch:
   - VLAN 10: Sales
   - VLAN 20: HR
2. Assigned PCs to VLANs:
   - PC0 to VLAN 10
   - PC1 to VLAN 20
3. Configured sub-interfaces on the router:
   - Sub-interface for VLAN 10: `192.168.10.1`
   - Sub-interface for VLAN 20: `192.168.20.1`
4. Set the default gateway on each PC:
   - PC0: `192.168.10.1`
   - PC1: `192.168.20.1`
5. Tested connectivity using the `ping` command.

## Screenshots
![image](https://github.com/user-attachments/assets/b6715ff1-1b39-4f98-b0ae-923eac01ce17)
![image](https://github.com/user-attachments/assets/a0051d69-044b-4c72-b66e-2324e3d58dda)

## Outcome
Successfully enabled communication between PCs in different VLANs.
