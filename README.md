# Wireshark
Network-traffic analyzer

### Overview

This project demonstrates the use of Wireshark to capture and analyze live network traffic in a controlled environment. The analysis focuses on DNS queries, TCP communication, ARP requests and replies, and HTTPS (TLS) traffic to understand how devices communicate over a network.


## Objectives

-  Analyze DNS request and response packets
-  Observe TCP three-way handshake
-  Capture live network packets
-  Study ARP request and reply process
-  Understand encrypted HTTPS communication using TLS
-  Interpret captured packets from a security perspective


## Tools 
- Kali Linux
- Wireshark
- VMware Workstation
- Firefox Web Browser


## Network Setup
- Operating System: Kali Linux
- Capture Interface: eth0
- Environment: VMware NAT Network


## Protocols Analyzed
- DNS
- TCP
- TLS/HTTPS
- ARP

## Analysis Performed:
## DNS Analysis
- Observed DNS queries and responses.
- Identified domain name resolution process.
- Analyzed A (IPv4) and AAAA (IPv6) DNS records.

## TCP Analysis
- Observed TCP three-way handshake.
  
  Verified connection establishment using:
- SYN
- SYN-ACK
- ACK

## TLS / HTTPS Analysis
- Observed TLS handshake.
  
  Identified:
- Client Hello
- Server Hello
- Certificate Exchange
- Key Exchange
- Encrypted Application Data

## ARP Analysis
- Captured ARP Request packets.
- Captured ARP Reply packets.
- Observed IP-to-MAC address resolution inside the local network.


## Key Findings
- DNS translates domain names into IP addresses.
- TCP establishes reliable communication using the three-way handshake.
- HTTPS encrypts communication after the TLS handshake.
- ARP resolves IP addresses to MAC addresses within the local network.
- Most modern websites communicate over encrypted HTTPS.


# Security Observations
- DNS traffic may reveal visited domains if not protected.
- HTTP traffic is unencrypted, whereas HTTPS encrypts transmitted data.
- ARP lacks authentication and is susceptible to ARP spoofing attacks.
- Encrypted TLS traffic protects sensitive information from interception.
