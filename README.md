# Multi-Site Pharmacy Network

A computer networks project that designs and simulates a multi-site network for a pharmacy organization using Cisco Packet Tracer.

The network connects a central Head Office with three pharmacy branches and provides communication between all locations while maintaining separate local area networks at each site.

The project implements dynamic routing, automatic IP addressing, DNS services, web services, local printing, and end-to-end communication between branches.

## Organization

The network is designed for a mid-sized pharmacy organization operating across multiple locations:

- Head Office
- Branch 1
- Branch 2
- Branch 3

The organization requires reliable communication between its locations to support operations such as:

- Inventory management
- Billing
- Administrative coordination
- Internal communication
- Access to shared network services
- Printing
- Access to the pharmacy web portal

Each location has its own local network, while the sites are connected through routers to allow communication across the organization.

## Project Aim

The main aim of this project is to design and simulate a functional multi-site network that allows the Head Office and pharmacy branches to communicate reliably.

The project focuses on:

- Multi-site network design
- LAN and WAN connectivity
- Dynamic routing
- Automatic IP configuration
- DNS services
- Web services
- Inter-branch communication
- Local device connectivity
- Network testing and troubleshooting
- Cisco Packet Tracer simulation

## Network Architecture

The network consists of four locations:

### Head Office

The Head Office contains:

- Router
- Network switch
- Desktop computers
- Network printer
- DHCP server
- DNS server
- Web server

The Head Office provides centralized DNS and web services that can be accessed by computers located in the pharmacy branches.

### Pharmacy Branches

Each pharmacy branch contains:

- Router
- Network switch
- Desktop computers
- Network printer
- DHCP server

Each branch operates its own LAN while maintaining connectivity with the Head Office and other locations through the WAN.

## Network Topology

The project combines two different network topologies.

### WAN Topology

The routers connecting the Head Office and pharmacy branches form a ring-based WAN topology.

This allows the different sites to communicate through the routed network.

### LAN Topology

Each individual location uses a star topology.

The network switch acts as the central device connecting:

- PCs
- Printers
- Servers
- Router

This design provides organized and manageable communication within each location.

## Network Devices

### Routers

Each site contains a router responsible for:

- Connecting the local network to other locations
- Forwarding traffic between networks
- Maintaining routing information
- Supporting dynamic routing using RIP
- Providing communication between the Head Office and pharmacy branches

The routers are interconnected through routed links with assigned IP addresses.

### Switches

Each site contains a network switch that connects the local devices within the LAN.

The switches allow communication between:

- Desktop computers
- Printers
- Servers
- Routers

### Desktop Computers

Desktop computers are used by employees for activities such as:

- Administrative tasks
- Inventory management
- Billing
- Accessing internal resources
- Accessing the pharmacy web portal

### Network Printers

Each location includes a network printer that can be accessed by devices within the local network.

The printers can be used for:

- Invoices
- Inventory lists
- Administrative documents
- Other pharmacy records

## Network Services

The network implements several services to support communication and network management.

### DHCP

Each location contains a dedicated DHCP server.

The DHCP servers automatically provide connected devices with:

- IP address
- Default gateway
- DNS server address

This reduces the need to manually configure IP settings on every computer.

All end devices are configured to obtain their network settings automatically through DHCP.

### DNS

A DNS server is located at the Head Office.

The DNS server stores the domain name associated with the pharmacy website and maps it to the IP address of the web server.

This allows users to access the pharmacy website using a domain name rather than entering the server IP address directly.

### Web Server

A web server is located at the Head Office.

The server hosts the pharmacy's internal web page, which can be accessed by computers located at both the Head Office and the pharmacy branches.

This demonstrates communication between different networks and access to centralized services.

## Routing

### RIP Dynamic Routing

The network uses Routing Information Protocol (RIP) for dynamic routing between the different sites.

RIP allows the routers to learn routes to other networks and maintain routing information automatically.

The routing tables were checked to confirm that the dynamic routes were correctly configured and that communication between the pharmacy locations was functioning.

## IP Addressing

Each site uses its own local network.

Devices receive their network configuration from the DHCP server at their location.

The network configuration includes:

- Device IP address
- Subnet information
- Default gateway
- DNS server address

Router interfaces are also assigned IP addresses to allow communication between the different networks.

## Connectivity Testing

Several tests were performed in Cisco Packet Tracer to verify that the network operates correctly.

### Inter-Branch Ping Test

A computer located at the Head Office successfully communicated with a computer located at a pharmacy branch using the `ping` command.

This confirmed that:

- Routing was functioning correctly
- The different networks could communicate
- The routers were forwarding traffic between locations

### Printer Connectivity Test

A computer successfully pinged the network printer located within its local network.

This confirmed that:

- The LAN was functioning correctly
- The printer was reachable
- Local network communication was working

### DNS Testing

The DNS server was configured with the pharmacy website record.

This allowed computers on the network to locate the web server through its configured domain name.

### Web Server Testing

Computers located in both the Head Office and the pharmacy branches successfully accessed the pharmacy website hosted on the Head Office web server.

This demonstrated that:

- DNS resolution was functioning
- The web server was reachable
- Inter-network communication was working

### DHCP Testing

Devices successfully received network configuration from their local DHCP servers.

The configuration included:

- IP address
- Default gateway
- DNS server

### RIP Routing Testing

The routing tables on the routers were examined to confirm that RIP had correctly learned the routes between the different networks.

## Technologies and Networking Concepts Used

- Cisco Packet Tracer
- Computer Networking
- LAN
- WAN
- TCP/IP
- IPv4 Addressing
- DHCP
- DNS
- HTTP / Web Services
- RIP Dynamic Routing
- Routers
- Network Switches
- Network Printers
- Client-Server Networking
- Star Topology
- Ring Topology
- Packet Testing
- Ping Testing
- Routing Tables

## Physical Connectivity

The network uses different connection types for the devices.

End devices are connected to network switches using Ethernet connections.

The routers provide communication between the different locations, while each switch acts as the communication center for devices within its local network.

The network design separates local communication within each branch from routed communication between pharmacy locations.

## Project Structure

```text
multi-site-pharmacy-network/
├── packet-tracer/
│   └── Net Project Router.pkt
├── report/
│   └── Net Summary.docx
└── README.md
```

## Main Files

- `Net Project Router.pkt` - Cisco Packet Tracer simulation containing the complete pharmacy network configuration
- `Net Summary.docx` - Project report containing the network design, device descriptions, topology, configuration information, screenshots, and connectivity testing
- `README.md` - Project overview and documentation

## How to Run the Project

1. Clone or download this repository.

2. Install Cisco Packet Tracer if it is not already installed.

3. Open the Packet Tracer project file:

   `packet-tracer/Net Project Router.pkt`

4. Allow the network topology to initialize.

5. Inspect the different locations:

   - Head Office
   - Branch 1
   - Branch 2
   - Branch 3

6. Check the DHCP configuration at each site.

7. Inspect the routing configuration on the routers.

8. Check the RIP routing tables.

9. Test connectivity between devices using the `ping` command.

10. Access the pharmacy website from a branch PC to verify DNS and web-server connectivity.

## Key Features

- Four interconnected pharmacy locations
- Head Office and three branches
- Separate LAN for each location
- Routed WAN connecting all locations
- RIP dynamic routing
- DHCP server at every location
- Central DNS server
- Central web server
- Automatic IP configuration
- Network printers
- Inter-branch communication
- Local LAN communication
- Centralized network services
- Successful connectivity testing

## Key Outcomes

The completed network demonstrated successful communication between the Head Office and pharmacy branches.

The project confirmed that:

- Devices within each LAN could communicate successfully.
- Devices could communicate across different pharmacy locations.
- RIP successfully provided dynamic routes between networks.
- DHCP automatically assigned network configuration to end devices.
- DNS successfully resolved the pharmacy website.
- Branch computers could access the web server located at the Head Office.
- Network printers were reachable from local computers.
- The combination of LAN and WAN networking supported communication across the organization.

## Notes

- The project was developed and tested using Cisco Packet Tracer.
- Each location operates its own LAN.
- The Head Office provides centralized DNS and web services.
- DHCP is configured separately at each location.
- RIP is used for dynamic routing between the pharmacy networks.
- The WAN uses a ring topology.
- Each individual LAN uses a star topology.
- Connectivity was verified using ping tests, routing tables, DHCP configuration, DNS resolution, and web-server access.

## Authors

- Ghala Alghamdi
- Hiba Amanulla
- Effat University
- Computer Science Department
- Course: CS2091 – Computer Networks
- Instructor: Dr. Mohmmad Nauman Amjad
