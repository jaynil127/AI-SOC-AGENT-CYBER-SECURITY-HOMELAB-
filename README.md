# AI-SOC-AGENT-CYBER-SECURITY-HOMELAB-
AI-powered SOC agent for detecting ICMP traffic, capturing packets with t-shark, generating alerts, and sending data to an AI webhook. Built in a cybersecurity home lab environment.
This project demonstrates a simple AI-powered Security Operations Center (SOC) agent built in a cybersecurity homelab environment. The tool captures network traffic using tshark, detects ICMP activity, generates alerts, and sends data to an AI webhook for further analysis.

## Project Overview

The AI SOC Agent monitors network traffic on a Kali Linux system and detects ICMP packets generated during simulated attack activity. In this lab setup, an Ubuntu machine acts as the attacker and sends ICMP ping requests to the Kali Linux system running the SOC agent.

The captured traffic is stored in PCAP format and analyzed to generate alerts that simulate basic SOC monitoring and incident detection workflows.

## Lab Environment

Attacker Machine: Ubuntu Linux  
Target Machine: Kali Linux (SOC Agent)  
Virtualization: VMware Virtual Lab  

Ubuntu sends ICMP ping requests to Kali Linux, and the AI SOC Agent monitors and analyzes the network traffic.

## Features

- Network traffic capture using tshark
- ICMP packet detection
- Packet capture stored in PCAP format
- Alert generation in JSON format
- Integration with AI webhook for automated analysis
- Basic SOC monitoring simulation

## Technologies Used

- Python
- Tshark
- Kali Linux
- Ubuntu Linux
- Network Packet Analysis
- Virtual Lab Environment

## Example Attack Simulation

Attacker (Ubuntu):

```
ping 192.168.1.10
```

SOC Agent (Kali Linux):

```
sudo python3 new_soc_capture.py
```

The SOC agent captures ICMP traffic, logs packet data, and generates alerts for analysis.

## Disclaimer

This project is created for educational and cybersecurity learning purposes only. The lab environment is used to simulate basic network monitoring and threat detection scenarios.
