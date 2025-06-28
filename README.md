# Computer Networks Laboratory 🌐

This repository contains Cisco Packet Tracer simulation files (.pkt) for various Computer Networks laboratory experiments. These simulations demonstrate fundamental networking concepts, protocols, and topologies commonly taught in computer networks courses.

## 📁 Repository Structure

All simulation files are located in the root directory and are organized by functionality:

### 🌐 Network Topologies (Basic Infrastructure)
- **Star with switch.pkt** - Star topology with central switch configuration
- **Bus With Switch.pkt** - Bus topology implementation using modern switches  
- **Ring with Hub.pkt** - Ring topology implementation with hub-based connectivity
- **Ring With Switch.pkt** - Ring topology using modern switch technology
- **Mesh with Switch.pkt** - Mesh topology using switched infrastructure
- **Hybrid.pkt** - Hybrid network topology combining multiple topology types

### 🔧 Network Services & Protocols

#### DHCP (Dynamic Host Configuration Protocol)
- **6.DHCP Server.pkt** - Dedicated DHCP server implementation and configuration
- **6.DCHP Server.pkt** - Alternative DHCP server setup (duplicate with typo)
- **dhcp using router.pkt** - Router-based DHCP services configuration

#### DNS (Domain Name System)
- **7.DNS Server.pkt** - Basic Domain Name System server setup
- **8.DNS using Switch.pkt** - DNS implementation in a switched network environment
- **9.DNS using router.pkt** - DNS configuration with router-based networks

#### VLAN (Virtual Local Area Networks)
- **VLAN.pkt** - Virtual Local Area Network configuration and inter-VLAN routing

### 🔗 Inter-LAN Connectivity & Routing
- **4.Two LANs Connection Using Router.pkt** - Connecting two Local Area Networks using a single router
- **5.Two LANs Using Two Router.pkt** - Inter-LAN communication using multiple routers for redundancy

---

## 🎯 Learning Path by Complexity

### 🟢 Beginner Level: Network Topologies
**Recommended Order:**
1. `Star with switch.pkt` - Start with the most common topology
2. `Bus With Switch.pkt` - Learn shared media concepts
3. `Ring With Switch.pkt` - Understand token-based communication
4. `Ring with Hub.pkt` - Compare hub vs switch implementations
5. `Mesh with Switch.pkt` - Explore redundant path concepts
6. `Hybrid.pkt` - Master complex mixed topologies

### � Intermediate Level: Network Services
**Recommended Order:**
1. `VLAN.pkt` - Virtual network segmentation
2. `6.DHCP Server.pkt` - Automatic IP address assignment
3. `dhcp using router.pkt` - Router-based DHCP implementation
4. `7.DNS Server.pkt` - Basic name resolution services
5. `8.DNS using Switch.pkt` - DNS in switched environments

### 🔴 Advanced Level: Complex Networking
**Recommended Order:**
1. `9.DNS using router.pkt` - DNS with routing integration
2. `4.Two LANs Connection Using Router.pkt` - Basic inter-LAN routing
3. `5.Two LANs Using Two Router.pkt` - Advanced multi-router scenarios

## 📊 Experiment Categories & Analysis

### 🔗 Network Topologies Analysis
| Topology Type | File | Devices Used | Complexity | Key Learning |
|---------------|------|-------------|------------|-------------|
| **Star** | `Star with switch.pkt` | Switch + PCs | ⭐ Beginner | Central point management |
| **Bus** | `Bus With Switch.pkt` | Switch + PCs | ⭐ Beginner | Shared media concepts |
| **Ring (Hub)** | `Ring with Hub.pkt` | Hub + PCs | ⭐⭐ Intermediate | Legacy ring implementation |
| **Ring (Switch)** | `Ring With Switch.pkt` | Switch + PCs | ⭐⭐ Intermediate | Modern ring with switches |
| **Mesh** | `Mesh with Switch.pkt` | Multiple Switches | ⭐⭐⭐ Advanced | Redundancy & fault tolerance |
| **Hybrid** | `Hybrid.pkt` | Mixed devices | ⭐⭐⭐ Advanced | Complex network design |

### 🌐 Network Services Analysis
| Service Type | Files Available | Implementation Method | Use Case |
|--------------|----------------|---------------------|----------|
| **DHCP** | `6.DHCP Server.pkt`<br>`6.DCHP Server.pkt`<br>`dhcp using router.pkt` | Dedicated Server<br>Router-based | Automatic IP assignment<br>Network configuration |
| **DNS** | `7.DNS Server.pkt`<br>`8.DNS using Switch.pkt`<br>`9.DNS using router.pkt` | Server-based<br>Switch integration<br>Router integration | Name resolution<br>Domain management |
| **VLAN** | `VLAN.pkt` | Switch configuration | Network segmentation<br>Security isolation |

### 🔀 Inter-LAN Connectivity Analysis
| Scenario | File | Router Count | Complexity | Key Concepts |
|----------|------|-------------|------------|-------------|
| **Basic Inter-LAN** | `4.Two LANs Connection Using Router.pkt` | 1 Router | ⭐⭐ Intermediate | Basic routing, subnetting |
| **Multi-Router LAN** | `5.Two LANs Using Two Router.pkt` | 2+ Routers | ⭐⭐⭐ Advanced | Routing protocols, redundancy |

## �️ Prerequisites

- **Cisco Packet Tracer** (Latest version recommended)
- Basic understanding of networking concepts
- Knowledge of IP addressing and subnetting
- Familiarity with Cisco IOS commands (for advanced configurations)

## �🚀 Getting Started

1. **Install Cisco Packet Tracer**
   - Download from [Cisco Networking Academy](https://www.netacad.com/courses/packet-tracer)
   - Register for a free account if needed

2. **Clone/Download Repository**
   ```bash
   git clone <repository-url>
   cd CN_Lab
   ```

3. **Choose Your Learning Path**
   - **Beginners**: Start with topology files (Star → Bus → Ring → Mesh → Hybrid)
   - **Intermediate**: Move to network services (VLAN → DHCP → DNS)
   - **Advanced**: Practice with inter-LAN routing scenarios

4. **Open Simulation Files**
   - Launch Cisco Packet Tracer
   - Open any `.pkt` file from the root directory
   - Follow the recommended learning path for structured progression

## 📚 Learning Objectives by Category

### � Network Topology Mastery
- **Primary Focus**: Physical and logical network design principles
- **Key Concepts**:
  - Topology advantages and disadvantages comparison
  - Device selection criteria (Hubs vs Switches)
  - Cable management and physical connectivity
  - Network scalability and performance considerations
  - Collision domains and broadcast domains

### 🌐 Network Services Implementation  
- **Primary Focus**: Essential networking protocols and services
- **Key Concepts**:
  - DHCP automatic IP assignment and lease management
  - DNS name resolution and domain management
  - VLAN network segmentation and security
  - Service integration and interoperability

### � Inter-LAN Routing & Connectivity
- **Primary Focus**: Advanced routing and network integration
- **Key Concepts**:
  - Static and dynamic routing configuration
  - Multi-router network design
  - Routing protocol implementation
  - Network redundancy and fault tolerance
  - Subnetting and VLSM (Variable Length Subnet Masking)

## 🔧 Common Commands by Implementation Type

### Basic Device Configuration (All Folders)
```cisco
Router> enable
Router# configure terminal
Router(config)# hostname R1
Router(config)# interface fastEthernet 0/0
Router(config-if)# ip address 192.168.1.1 255.255.255.0
Router(config-if)# no shutdown
```

### Switch Configuration (Exp3/ - Topologies)
```cisco
Switch> enable
Switch# configure terminal
Switch(config)# hostname SW1
Switch(config)# interface fastEthernet 0/1
Switch(config-if)# description "Connection to PC1"
Switch(config-if)# no shutdown
```

### DHCP Configuration (Root + untitled folder/)
```cisco
Router(config)# ip dhcp pool LAN_POOL
Router(dhcp-config)# network 192.168.1.0 255.255.255.0
Router(dhcp-config)# default-router 192.168.1.1
Router(dhcp-config)# dns-server 8.8.8.8
Router(dhcp-config)# lease 7
```

### VLAN Configuration (Root Directory)
```cisco
Switch(config)# vlan 10
Switch(config-vlan)# name SALES
Switch(config)# vlan 20
Switch(config-vlan)# name ENGINEERING
Switch(config)# interface fastEthernet 0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 10
```

### DNS Configuration (DNS Services)
```cisco
Router(config)# ip dns server
Router(config)# ip host server1.local 192.168.1.10
Router(config)# ip name-server 8.8.8.8
```

### Routing Configuration (Inter-LAN scenarios)
```cisco
Router(config)# router ospf 1
Router(config-router)# network 192.168.1.0 0.0.0.255 area 0
Router(config-router)# network 192.168.2.0 0.0.0.255 area 0
```

## 📖 Category-Wise Lab Exercise Guidelines

### � Network Topology Practice (Beginner Level)
1. **Begin with Star Topology** - `Star with switch.pkt`
   - Understand central switch concept
   - Configure basic IP addressing
   - Test connectivity between devices

2. **Progress to Bus Topology** - `Bus With Switch.pkt`
   - Learn shared media concepts
   - Observe collision domain behavior
   - Compare with star topology performance

3. **Explore Ring Topologies** - Both hub and switch versions
   - `Ring with Hub.pkt` - Legacy token-passing concepts
   - `Ring With Switch.pkt` - Modern ring implementation
   - Compare hub vs switch implementations and analyze fault tolerance

4. **Master Complex Topologies** - Mesh and Hybrid
   - `Mesh with Switch.pkt` - Design redundant paths and implement load balancing
   - `Hybrid.pkt` - Configure complex mixed topologies
   - Implement load balancing
   - Configure spanning tree protocol

### 🌐 Network Services Implementation (Intermediate Level)
1. **Implement VLANs** - `VLAN.pkt`
   - Create multiple VLANs for network segmentation
   - Configure inter-VLAN routing
   - Test VLAN isolation and communication

2. **Configure DHCP Services**
   - Start with `6.DHCP Server.pkt` for dedicated server approach
   - Progress to `dhcp using router.pkt` for router-based DHCP
   - Compare implementation approaches and performance
   - Note: `6.DCHP Server.pkt` is a duplicate file with typo

3. **Setup DNS Services**
   - Begin with `7.DNS Server.pkt` for basic DNS server configuration
   - Advance to `8.DNS using Switch.pkt` for switched network DNS
   - Master `9.DNS using router.pkt` for router-integrated DNS
   - Test name resolution functionality across different implementations

### 🔀 Inter-LAN Routing Practice (Advanced Level)
1. **Basic Inter-LAN Connectivity** - `4.Two LANs Connection Using Router.pkt`
   - Configure single router for dual LAN connectivity
   - Implement subnetting and basic routing
   - Test inter-LAN communication and troubleshoot issues

2. **Advanced Multi-Router Scenarios** - `5.Two LANs Using Two Router.pkt`
   - Design redundant routing paths
   - Implement routing protocols (RIP, OSPF)
   - Configure network redundancy and failover

## 🔍 Category-Specific Troubleshooting Tips

### � Network Topology Issues
- **Physical Layer**: Check cable types (straight-through vs crossover) and physical connections
- **Data Link Layer**: Verify switch configurations, port status, and MAC address tables
- **Spanning Tree**: Resolve loops in redundant topologies, check STP convergence
- **Performance**: Monitor collision domains, broadcast domains, and network utilization

### 🌐 Network Services Issues
- **DHCP Problems**: 
  - Check DHCP pool configurations and scope
  - Verify excluded IP addresses and lease duration
  - Test DHCP lease renewal and release processes
  - Monitor DHCP server logs for conflicts

- **DNS Issues**:
  - Validate DNS server IP configurations on clients
  - Check forward and reverse lookup zones
  - Test name resolution with nslookup and ping commands
  - Verify DNS server reachability and service status

- **VLAN Problems**:
  - Verify VLAN assignments on switch ports
  - Check trunk configurations and allowed VLANs
  - Test inter-VLAN routing and gateway configurations
  - Monitor VLAN database consistency

### � Inter-LAN Routing Issues
- **Routing Problems**:
  - Check routing table entries with `show ip route`
  - Verify next-hop reachability and interface status
  - Test routing protocol convergence and updates
  - Analyze network topology for routing loops

- **Multi-Router Configuration**:
  - Validate routing protocol configurations (OSPF, RIP)
  - Check network advertisements and area configurations
  - Monitor routing updates and LSA propagation
  - Test failover scenarios and convergence time

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

## 📋 Quick Reference Guide

### 🎯 File Selection Guide
| **If you want to learn...** | **Start with these files** | **Difficulty** |
|----------------------------|---------------------------|---------------|
| **Basic networking concepts** | `Star with switch.pkt` → `Bus With Switch.pkt` | ⭐ Beginner |
| **Network topologies** | `Ring with Hub.pkt` → `Ring With Switch.pkt` → `Mesh with Switch.pkt` | ⭐⭐ Intermediate |
| **Advanced topologies** | `Hybrid.pkt` | ⭐⭐⭐ Advanced |
| **Automatic IP assignment** | `6.DHCP Server.pkt` → `dhcp using router.pkt` | ⭐⭐ Intermediate |
| **Name resolution** | `7.DNS Server.pkt` → `8.DNS using Switch.pkt` → `9.DNS using router.pkt` | ⭐⭐ Intermediate |
| **Network segmentation** | `VLAN.pkt` | ⭐⭐ Intermediate |
| **Inter-network routing** | `4.Two LANs Connection Using Router.pkt` → `5.Two LANs Using Two Router.pkt` | ⭐⭐⭐ Advanced |

### 🚀 Recommended Learning Sequence
```
Phase 1: Topology Fundamentals (1-2 weeks)
├── Star with switch.pkt
├── Bus With Switch.pkt  
├── Ring with Hub.pkt
├── Ring With Switch.pkt
├── Mesh with Switch.pkt
└── Hybrid.pkt

Phase 2: Network Services (2-3 weeks)  
├── VLAN.pkt
├── 6.DHCP Server.pkt
├── dhcp using router.pkt
├── 7.DNS Server.pkt
├── 8.DNS using Switch.pkt
└── 9.DNS using router.pkt

Phase 3: Advanced Routing (2-3 weeks)
├── 4.Two LANs Connection Using Router.pkt
└── 5.Two LANs Using Two Router.pkt
```

### 📊 File Status & Notes
| File Name | Status | Notes |
|-----------|--------|-------|
| `6.DCHP Server.pkt` | ⚠️ Duplicate | Same as `6.DHCP Server.pkt` (contains typo in filename) |
| `6.DHCP Server.pkt` | ✅ Primary | Use this version for DHCP server learning |
| All other `.pkt` files | ✅ Active | Ready for use in laboratory exercises |
