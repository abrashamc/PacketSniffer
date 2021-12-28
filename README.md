# Packet Sniffer

Sniff traffic from wired/wireless NIC.

## Run
- sudo python3 network_app.py
- Specify: 
  - interface (e.g. enp0s8)
  - number of packets to capture (0 is infinity)
  - timeout (in seconds)
  - protocol to filter (0 is all)

## Notes
Current supported filters - ARP, BOOTP, ICMP.\
Tweak script to add any protocol (TCP, UDP etc.)

## Dependency
- [Scapy](https://scapy.readthedocs.io/en/latest/)

## Example
Ping server and capture icmp calls

![Preview](https://i.imgur.com/hL25SFn.png)

Log file -\
Time: 2021-12-28 16:51:09.717259 Protocol: ICMP SMAC: 65:3f:11:7a:b4:rg DMAC: 14:55:76:45:23:a1\
Time: 2021-12-28 16:51:09.717735 Protocol: ICMP SMAC: 14:55:76:45:23:a1 DMAC: 65:3f:11:7a:b4:rg\
Time: 2021-12-28 16:51:09.818930 Protocol: ICMP SMAC: 14:55:76:45:23:a1 DMAC: 65:3f:11:7a:b4:rg\
Time: 2021-12-28 16:51:09.819566 Protocol: ICMP SMAC: 65:3f:11:7a:b4:rg DMAC: 14:55:76:45:23:a1\
Time: 2021-12-28 16:51:10.717741 Protocol: ICMP SMAC: 65:3f:11:7a:b4:rg DMAC: 14:55:76:45:23:a1\
Time: 2021-12-28 16:51:10.718216 Protocol: ICMP SMAC: 14:55:76:45:23:a1 DMAC: 65:3f:11:7a:b4:rg\
Time: 2021-12-28 16:51:10.843485 Protocol: ICMP SMAC: 14:55:76:45:23:a1 DMAC: 65:3f:11:7a:b4:rg\
Time: 2021-12-28 16:51:10.843993 Protocol: ICMP SMAC: 65:3f:11:7a:b4:rg DMAC: 14:55:76:45:23:a1\
Time: 2021-12-28 16:51:11.719705 Protocol: ICMP SMAC: 65:3f:11:7a:b4:rg DMAC: 14:55:76:45:23:a1\
Time: 2021-12-28 16:51:11.720238 Protocol: ICMP SMAC: 14:55:76:45:23:a1 DMAC: 65:3f:11:7a:b4:rg\
