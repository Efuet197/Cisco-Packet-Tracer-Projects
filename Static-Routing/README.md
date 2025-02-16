# Static Routing

## Objective
Configure static routing between two routers to connect two separate networks.

## Steps
1. Assigned IP addresses:
   - PC0: `192.168.1.1`
   - PC1: `192.168.2.1`
   - Router0 interface: `192.168.1.254`
   - Router1 interface: `192.168.2.254`
   - Router0 to Router1 link: `10.0.0.1` (Router0) and `10.0.0.2` (Router1)
2. Configured static routes on both routers:
   - On Router0: `ip route 192.168.2.0 255.255.255.0 10.0.0.2`
   - On Router1: `ip route 192.168.1.0 255.255.255.0 10.0.0.1`
3. Tested connectivity using the `ping` command.

## Screenshots
![image](https://github.com/user-attachments/assets/a52ee7cc-59de-4434-a1b2-1de87a8faf8f)
![image](https://github.com/user-attachments/assets/aea6d449-9754-4954-93d6-e3362296fd0f)

## Outcome
Successfully established communication between the two networks.
