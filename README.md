Task 1 - Port Scanning

Tools Used
- Nmap
- Command Prompt
- Wireshark

 Objective
Scan local network for open ports and understand potential security exposure.

 Commands Used:
     ipconfig (To find my local IP)
     nmap -sS 192.168.1.0/24 (To scan all devices on my network for TCP ports)
    
RESULTS
 IP addresses and open ports found and their screenshots are attatched in this repository.
 Also, I analyzed packet capture with wireshark and I applied filters like tcp.port == 80  
 tcp.port == 22  for SSH and tcp.port == 445  for SMB.


SECURITY OBSERVATIONS
Port 80 is open on 192.168.1.1 – I found it as the router with web interface

Ports 135, 139, 445 on 192.168.1.6 are associated with Windows SMB services, which are common targets for attacks.

Devices 192.168.1.2, .3, and .5 had no open ports reported or were filtered.

 
 What I Learned
  How to use nmap  for a stealth scan on a subnet

  How to interpret scan results and identify service names

  Basic understanding of open ports, filtered ports, and their risks

  A quick look into MAC address vendor identification

