# SSH Brute-Force Detection Lab

## Objective
Detect SSH brute-force login attempts using Ubuntu Server logs.

## Tools Used
- Ubuntu Server 26.04 LTS
- Kali Linux 2025.3
- VirtualBox
- OpenSSH
- journalctl

## Network Setup

Kali Linux (192.168.56.102)
        |
        | SSH Login Attempts
        v
Ubuntu Server (192.168.56.101)
        |
        v
Authentication Logs
        |
        v
SOC Detection

## Commands Used

ip a

ping 192.168.56.101

ssh thunder@192.168.56.101

sudo journalctl -u ssh | grep "failed"

## Results

Multiple failed login attempts were generated and detected in Ubuntu authentication logs.

## Skills Demonstrated

- Linux Administration
- SSH Configuration
- Log Analysis
- SOC Monitoring
- Incident Detection
- Threat Hunting
