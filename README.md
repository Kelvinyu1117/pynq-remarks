# PYNQ Remarks
This repository contains the remarks for using PYNQ board for AI applications

## Setup

### Hardware Setup
https://pynq.readthedocs.io/en/latest/getting_started/pynq_z2_setup.html

### Network Configuration

- Connected to Ethernet port of the PC

- Connected to the routing table

#### Connected to Ethernet port of the PC

- Local network

  - Assign static address to the port of the PC
  
  | IP          | Subnet Mask   |
  |-------------|---------------|
  | 192.168.2.x | 255.255.255.0 |
  
  - Using SSH tunnel for port forwarding, map traffic from the remote port to local port if needed
  
    `ssh -L localhost:<host-port>:localhost:<remote-port> userName@<remote-ip>`

- Use PC as a bridge

