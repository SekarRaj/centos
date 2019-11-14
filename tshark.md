# Network packet capture

`tshark` is the cli for wireshark. 

```bash
# Capture TCP/UDP traffic
$ tshark -i Ethernet -f "tcp or udp 68" 

# Capture in pcap format
$ tshark -i Ethernet -f "udp port 68" -F pcap -w packet.pcap
$ tshark -r packet.pcap -V
```
