# Packet Sniffer

Connect to remote servers through SSHv2 protocol and execute pre-defined commands.\
Can be used for software provisioning, configuration management, and application-deployment enabling infrastructure as code.  
It runs on many Unix-like systems, and can configure both Unix-like systems and Microsoft Windows.

## Run
- sudo python3 network_app.py

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

## Dependency
- [Scapy](https://scapy.readthedocs.io/en/latest/)