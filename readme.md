*This project has been created as part of the 42 curriculum by afournie.*

# NetPractice

## Description

NetPractice is a pedagogical project from the 42 curriculum focused on network
configuration and IP addressing. The goal of the project is to understand and
apply core networking fundamentals — subnetting, routing, and device
configuration — through a series of increasingly difficult exercises.

Each exercise presents a small network topology made of hosts, switches, and
routers. The topology contains errors or missing information (incorrect IP
addresses, wrong subnet masks, missing routes, misconfigured gateways, etc.).
The objective is to fix the configuration of each network element so that all
devices on the topology can communicate correctly with one another, respecting
the constraints given for each level (available address ranges, number of
usable hosts per subnet, etc.).

This project does not involve writing code: it is entirely about understanding
and reasoning through networking concepts using the graphical training
interface provided by 42.

## Instructions

### Requirements

- A Linux or macOS environment (the training interface is a graphical
  application).
- The NetPractice archive/toolkit provided by 42, containing the `run.sh`
  script and the exercise levels.

### Running the training interface

From the root of the project, launch the interface with:

```bash
./run.sh
```

This opens the graphical interface where the network topology for the
selected level is displayed. Each host, switch, and router can be selected to
edit its configuration (IP address, subnet mask, default gateway, routing
table entries, etc.).

### Solving a level

1. Select a level from the interface.
2. Analyze the given topology and the constraints (address range, number of
   hosts, etc.).
3. Click on each network interface or device to edit its configuration.
4. Use the "Check" (or equivalent) button in the interface to verify that all
   hosts can reach each other.
5. Once the level is validated, export the configuration.

### Exporting configurations

Each validated level must be exported to a configuration file using the
export option provided by the interface (usually a "Save"/"Export" button).
The exported file corresponds to the solved topology for that level.

### Submission

- The project must be submitted with **10 exported configuration files**, one
  per level, placed **at the root of the repository**.
- File naming should follow the convention required by the interface/subject
  (e.g. `lvl1.net`, `lvl2.net`, ... `lvl10.net`).
- Make sure every configuration file is actually validated (green/OK status)
  in the interface before exporting and committing it.

## Resources

### Networking concepts studied

- TCP/IP addressing (IPv4)
- Subnetting and subnet masks (CIDR notation)
- Network and broadcast addresses, usable host ranges
- Default gateways
- Static routing and routing tables
- Routers vs. switches: roles and differences
- OSI model layers (particularly Layer 2 – Data Link and Layer 3 – Network)
- ARP (Address Resolution Protocol) basics

### References

- [RFC 791 – Internet Protocol](https://datatracker.ietf.org/doc/html/rfc791)
- [RFC 950 – Internet Standard Subnetting Procedure](https://datatracker.ietf.org/doc/html/rfc950)
- [Cisco Networking Basics](https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/networking-basics.html)
- [Subnetting practice tool – subnetting.net](https://subnetting.net/)
- [OSI Model explained – Cloudflare Learning Center](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)

### AI usage disclosure

AI assistance (Claude) was used during this project for:

- Reviewing and improving the wording of this README file.

AI was **not** used to solve the NetPractice exercises themselves: all
topology configurations were designed, tested, and validated manually through
the training interface, in accordance with the project's rules.
