# SSH Brute-force Log Analysis

## Log Source
Linux system authentication logs (`/var/log/auth.log`)

## Attack Overview
An SSH brute-force attack involves repeated login attempts using
multiple username and password combinations to gain unauthorized access.

## Sample Log Evidence
Failed password for invalid user admin from 192.168.1.100 port 44532 ssh2
Failed password for root from 192.168.1.100 port 44540 ssh2


## Indicators of Compromise (IOCs)
- Source IP: 192.168.1.100
- Multiple failed login attempts
- Common usernames targeted (root, admin)

## Analysis
- Repeated authentication failures from the same IP
- Short time interval between attempts
- Indicates automated brute-force activity

## SOC Response Actions
- Block source IP at firewall
- Enable fail2ban
- Generate high-severity alert
- Monitor for lateral movement
