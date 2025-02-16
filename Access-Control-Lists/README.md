# ACL Configuration

## Objective
Use Access Control Lists (ACLs) to restrict traffic between networks.

## Steps
1. Created an ACL to block traffic from PC0 to PC1:
   - `access-list 100 deny ip 192.168.1.0 0.0.0.255 192.168.2.0 0.0.0.255`
   - `access-list 100 permit ip any any`
2. Applied the ACL to the router interface:
   - `interface GigabitEthernet0/1`
   - `ip access-group 100 in`
3. Tested connectivity using the `ping` command.

## Screenshots
![image](https://github.com/user-attachments/assets/f6225170-27be-4e5f-b78d-8a9c9e81afc5)
![image](https://github.com/user-attachments/assets/10708e38-5f05-407b-a9cd-b07e34a24bf7)

## Outcome
Successfully blocked traffic from PC0 to PC1 while allowing other traffic.
