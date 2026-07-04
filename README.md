# Home Network Topology Lab

## Project Overview

I created this home network topology lab to strengthen my networking fundamentals and improve my understanding of how network traffic flows from a Security Operations Centre (SOC) analyst's perspective. This project also gave me hands-on experience with basic network design and traffic analysis using Wireshark.

## Objectives

- Build a basic home network topology.
- Understand the role of the ISP modem, firewall, and wireless router.
- Capture and analyze network traffic using Wireshark.
- Understand how traffic flows from a client device to a web server.
- Demonstrate foundational networking knowledge relevant to SOC analysis.

## Network Topology

The network consists of:

- ISP Modem
- Firewall
- Wireless Router (192.168.1.1)
- Laptop (Wireshark – 192.168.1.5)
- Smartphone (192.168.1.8)
- Smart TV (192.168.1.10)

## Network Traffic Analysis

### Traffic Flow

1. A user requests a web page.
2. The client performs a DNS lookup to resolve the web server's IP address.
3. A TCP three-way handshake (SYN → SYN-ACK → ACK) is established between the client and the web server.
4. The wireless router forwards the packet.
5. The firewall inspects the traffic.
6. The ISP modem sends the traffic to the Internet.
7. The web server processes the HTTP/HTTPS request.
8. The response is returned to the client device.

### Wireshark Observations

During packet capture, I was able to observe:

- ARP requests and replies for local device communication.
- DNS queries used to resolve domain names.
- The TCP three-way handshake establishing a connection before data transfer.
- HTTP/HTTPS traffic between the client and the web server.
- Packet flow between devices on the local network and the Internet.

## Security Considerations

This lab highlights several basic security concepts:

- Firewalls help filter and monitor network traffic.
- IP addresses identify devices connected to the network.
- Routers perform Network Address Translation (NAT) to allow multiple devices to share a public IP address.
- Keeping home devices updated helps reduce security risks.
- Strong Wi-Fi security, such as WPA2 or WPA3, should always be enabled.

## What I Learned

This project strengthened my understanding of basic networking concepts, including IP addressing, DNS resolution, TCP/IP communication, packet flow, and Network Address Translation (NAT). Using Wireshark allowed me to observe how devices communicate across a network and reinforced the importance of network traffic analysis in a Security Operations Centre (SOC) environment.  This lab helped me connect networking theory with practical, hands-on experience.



