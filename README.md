# Computer Networks Laboratory 🌐

This repository contains Cisco Packet Tracer simulation files for various Computer Networks laboratory experiments. These simulations demonstrate fundamental networking concepts, protocols, and topologies commonly taught in computer networks courses.

## 📁 Repository Structure

### Main Directory
- **4.Two LANs Connection Using Router.pkt** - Connecting two Local Area Networks using a single router
- **5.Two LANs Using Two Router.pkt** - Inter-LAN communication using multiple routers
- **6.DCHP Server.pkt** / **6.DHCP Server.pkt** - DHCP server implementation and configuration
- **7.DNS Server.pkt** - Domain Name System server setup
- **8.DNS using Switch.pkt** - DNS implementation in a switched network
- **9.DNS using router.pkt** - DNS configuration with router-based networks
- **VLAN.pkt** - Virtual Local Area Network configuration
- **dhcp using router.pkt** - DHCP services through router configuration

### Experiment 3 - Network Topologies (`Exp3/`)
- **Bus With Switch.pkt** - Bus topology implementation using switches
- **Hybrid.pkt** - Hybrid network topology combining multiple topology types
- **Mesh with Switch.pkt** - Mesh topology using switched infrastructure
- **Ring with Hub.pkt** - Ring topology implementation with hub-based connectivity
- **Ring With Switch.pkt** - Ring topology using modern switch technology
- **Star with switch.pkt** - Star topology with central switch configuration

### Experiments 4 & 5 - Multi-LAN Configurations (`Exp4 & 5/`)
- **4.2 LAN using Router.pkt** - Dual LAN setup with single router
- **5.2 LAN using 2 Routers.pkt** - Two LAN networks connected via dual router setup

### Additional Experiments (`untitled folder/`)
- **bus topology.pkt** - Basic bus network topology
- **dhcp server implementation.pkt** - Comprehensive DHCP server setup
- **dhcp using router.pkt** - Router-based DHCP configuration
- **dns using router.pkt** - DNS services through router
- **dns.pkt** - Basic DNS server configuration
- **dns_using server.pkt** - Dedicated DNS server implementation
- **hybrid.pkt** - Hybrid topology demonstration
- **mesh topology.pkt** - Full mesh network implementation
- **realdns_router.pkt** - Real-world DNS with router configuration
- **ring topology with switch.pkt** - Ring network using switches
- **star topology.pkt** - Basic star topology implementation
- **two lans connection using router.pkt** - Dual LAN router connection
- **two lans using two router.pkt** - Multi-router LAN interconnection

## 🛠️ Prerequisites

- **Cisco Packet Tracer** (Latest version recommended)
- Basic understanding of networking concepts
- Knowledge of IP addressing and subnetting
- Familiarity with Cisco IOS commands (for advanced configurations)

## 🚀 Getting Started

1. **Install Cisco Packet Tracer**
   - Download from [Cisco Networking Academy](https://www.netacad.com/courses/packet-tracer)
   - Register for a free account if needed

2. **Clone/Download Repository**
   ```bash
   git clone <repository-url>
   cd CN-Lab
   ```

3. **Open Simulation Files**
   - Launch Cisco Packet Tracer
   - Open any `.pkt` file from the repository
   - Explore the network topology and configurations

## 📚 Learning Objectives

### Network Topologies
- Understand different network topologies (Star, Bus, Ring, Mesh, Hybrid)
- Compare advantages and disadvantages of each topology
- Implement topologies using various networking devices

### Network Services
- **DHCP (Dynamic Host Configuration Protocol)**
  - Automatic IP address assignment
  - Network configuration management
  - Server and router-based implementations

- **DNS (Domain Name System)**
  - Name resolution services
  - DNS server configuration
  - Integration with network infrastructure

### Inter-networking
- **LAN-to-LAN Communication**
  - Router-based connectivity
  - Multi-router networks
  - Routing protocols and configurations

- **VLANs (Virtual Local Area Networks)**
  - Network segmentation
  - VLAN configuration and management
  - Inter-VLAN routing

## 🔧 Common Commands and Configurations

### Basic Router Commands
```cisco
Router> enable
Router# configure terminal
Router(config)# interface fastEthernet 0/0
Router(config-if)# ip address 192.168.1.1 255.255.255.0
Router(config-if)# no shutdown
```

### DHCP Configuration
```cisco
Router(config)# ip dhcp pool LAN_POOL
Router(dhcp-config)# network 192.168.1.0 255.255.255.0
Router(dhcp-config)# default-router 192.168.1.1
Router(dhcp-config)# dns-server 8.8.8.8
```

### VLAN Configuration
```cisco
Switch(config)# vlan 10
Switch(config-vlan)# name SALES
Switch(config)# interface fastEthernet 0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 10
```

## 📖 Lab Exercise Guidelines

1. **Start with Basic Topologies** - Begin with simple star and bus topologies
2. **Progress to Complex Networks** - Move to hybrid and mesh configurations
3. **Implement Services** - Add DHCP and DNS services to your networks
4. **Test Connectivity** - Use ping and traceroute to verify network functionality
5. **Document Configurations** - Keep notes of IP schemes and device configurations

## 🔍 Troubleshooting Tips

- **Check Physical Connections** - Ensure all cables are properly connected
- **Verify IP Configurations** - Confirm correct IP addresses and subnet masks
- **Test Layer by Layer** - Use OSI model approach for systematic troubleshooting
- **Use Packet Tracer Tools** - Utilize built-in simulation and real-time modes
- **Check Routing Tables** - Verify routing information on routers

## 📝 Additional Resources

- [Cisco Packet Tracer Tutorials](https://www.netacad.com/courses/packet-tracer)
- [Cisco IOS Command Reference](https://www.cisco.com/c/en/us/support/ios-nx-os-software/ios-software-releases-122-mainline.html)
- [Computer Networks Fundamentals](https://www.coursera.org/learn/computer-networks)

## 📄 License

This project is for educational purposes. Cisco Packet Tracer files are meant for learning and practicing network configurations.

## 👥 Authors

Computer Networks Laboratory Course Materials

---

**Note**: These simulation files are designed for educational purposes and may require adjustments based on specific network requirements or newer software versions.
