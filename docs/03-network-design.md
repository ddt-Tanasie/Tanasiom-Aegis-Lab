# Network Design

## Lab Network

The lab environment uses a VirtualBox host-only network.

Network range:

192.168.56.0/24

This network allows the virtual machines to communicate with each other while remaining isolated from the external internet.

## Example IP assignments

Kali Linux
192.168.56.101

Ubuntu Server
192.168.56.104

Metasploitable
192.168.56.105

## Security Model

The environment simulates a typical internal network scenario in which an attacker has gained internal network access.

The Kali Linux machine represents a security tester performing an authorised internal security assessment.

This setup allows demonstration of:

- internal reconnaissance
- service discovery
- vulnerability identification
- exploitation paths
