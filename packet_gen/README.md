# Packet Generator

Packet generator is a binary file that is generated for nIDS test purpose. It has the following features:

1. Ethernet
2. ARP
3. MACsec
4. IPv4
5. Pcap replay
6. ICMP

PCAP replay can either be replayed at configured period or can be replayed by identifying exactly time difference
between the two packets and using that to acheive exact Inter Packet Gap.

## Requirements

Require the below OS and the jsoncpp-dev installed.

1. Ubuntu 23.10
2. libjsoncpp-dev

## How to use it

1. Packet_gen.json contains the configuration data for each packet formats.
2. Only one packet type can be set at once.


```bash
chmod +x packet_gen
sudo ./packet_gen -f packet_gen.json
```

