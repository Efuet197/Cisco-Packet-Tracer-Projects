# NAT Configuration

## Objective
Configure NAT to allow internal PCs to access the internet.

## Steps
1. Set up a router with NAT.
2. Configured access lists and NAT overload:
   - `access-list 1 permit 192.168.1.0 0.0.0.255`
   - `ip nat inside source list 1 interface GigabitEthernet0/1 overload`
3. Assigned IP addresses:
   - Internal network: `192.168.1.0/24`
   - External network: `200.0.0.0/24`
4. Tested connectivity to an external server.

## Screenshots
![image](https://github.com/user-attachments/assets/f5b067c0-08cf-4c7b-bf64-c3547af78bc2)
![image](https://github.com/user-attachments/assets/cb2baef9-6e37-4de0-b9db-2b5165422e4c)

## Outcome
Internal PCs could successfully access the external network.
