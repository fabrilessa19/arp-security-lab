# ARP Security Lab

## Overview

This project documents practical experiments to understand how the Address Resolution Protocol (ARP) works inside a local network.

The goal of this lab is to observe ARP requests and replies, analyze the ARP cache, and understand how ARP can be abused in attacks such as ARP spoofing.

All experiments were performed using virtual machines in a controlled lab environment.

---

## What is ARP?

The Address Resolution Protocol (ARP) is responsible for mapping IP addresses to MAC addresses in a local network.

When a device wants to send a packet to another device on the same network, it must know the destination MAC address. If the MAC address is unknown, the system sends an ARP request asking:

"Who has this IP address?"

The device that owns that IP address responds with an ARP reply containing its MAC address.

After this process, the sender stores the information in the ARP cache and can send packets normally.

---

## Lab Environment

This lab was performed using the following environment:

Virtualization platform

* VirtualBox

Operating systems

* Kali Linux (attacker / analysis machine)
* AlmaLinux (target machine)

Both machines are connected to the same virtual network.

---

## Network Configuration

Kali Linux
IP address: 192.168.56.100

AlmaLinux
IP address: 192.168.56.102

Both machines are located in the same LAN segment.

---

## Tools Used

The following tools were used during the experiments:

* tcpdump
* ping
* ip command
* Linux networking utilities

These tools allow observation and analysis of ARP traffic.

---

## Experiments

This project contains the following experiments:

### 1. ARP Basics

Observation of ARP request and reply messages when two hosts communicate in the same network.

### 2. ARP Cache Analysis

Analysis of how ARP entries are stored in the ARP table and how the cache behaves.

### 3. ARP Spoofing Concept

Explanation of how attackers can manipulate ARP messages to perform a Man-in-the-Middle attack.

---

## Learning Goals

The objective of this project is to understand:

* How ARP works in local networks
* How devices resolve MAC addresses from IP addresses
* How ARP traffic can be captured and analyzed
* Basic concepts behind ARP spoofing attacks

---

## Future Improvements

Possible improvements for this project include:

* Demonstrating a practical ARP spoofing attack
* Capturing packets using Wireshark
* Building a small Python script to detect ARP poisoning
* Expanding the lab with more hosts

---

## Disclaimer

All experiments were performed in a controlled lab environment using virtual machines.

These techniques are documented for educational and cybersecurity learning purposes only.
