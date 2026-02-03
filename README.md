## Linux Network Security Hardening using UFW

## Overview

This project demonstrates basic network security hardening on a Linux system by configuring firewall rules using UFW (Uncomplicated Firewall).
The goal is to reduce the attack surface by allowing only essential services and blocking unused or risky ports.

## Objectives

Enable and configure a host-based firewall

Implement a default deny inbound security policy

Allow only required network services

Block unused and insecure ports

Verify firewall enforcement using controlled port scanning

## Tools & Technologies

Kali Linux

UFW (Uncomplicated Firewall)

Nmap

## Firewall Configuration

The following security controls were implemented:

Enabled UFW firewall

Set default policy:

Deny all incoming traffic

Allow all outgoing traffic

Allowed essential services:

SSH (22)

HTTP (80)

HTTPS (443)

Blocked unused / insecure ports:

FTP (21)

Telnet (23)

Enabled firewall logging

## Verification & Testing

Firewall rules were validated by performing controlled Nmap scans against the local system.

A scan on port 21 (FTP) returned a closed state

This confirms that the firewall rules are actively blocking unauthorized access

Verification was performed on the local loopback address (127.0.0.1) in a safe lab environment

## Screenshots

The following screenshots document the configuration and verification process:

1_ufw_firewall_enabled.png – Firewall enabled successfully

2_ufw_rules_configuration.png – Allowed and denied firewall rules

3_nmap_blocked_port_verification.png – Nmap scan confirming blocked port

## Outcome

Reduced exposed network services

Prevented access to unused and insecure ports

Implemented real-world Linux firewall controls

Gained hands-on experience in network security fundamentals

## Key Learnings

Firewall rule design and enforcement

Difference between allowed and denied traffic

Using Nmap to validate security controls

Understanding host-based network security

## Disclaimer

This project was performed in a local and controlled environment for learning purposes only.
No external systems were scanned.

