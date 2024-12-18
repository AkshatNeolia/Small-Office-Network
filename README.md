# Small Office Networks (Computer Networks)

## Project Overview

The project focuses on the design and implementation of a **Small Office Network** to address network congestion and optimize performance through the use of VLAN segmentation, inter-VLAN routing, and other networking techniques.

### Objectives
- To design a secure and efficient network for a small office environment.
- Implement VLANs to enhance security and manage network traffic.
- Configure inter-VLAN routing for seamless communication between departments.
- Test and validate network performance for scalability and reliability.

## Features
- **VLAN Segmentation**: Isolation of network traffic for Admin/IT, Finance/HR, and Customer Service/Reception.
- **Inter-VLAN Routing**: Configured using Layer 3 switching and sub-interfaces on routers.
- **DHCP Server Configuration**: Automated IP address assignment within VLANs.
- **Wireless Network Setup**: Department-specific SSIDs with VLAN tagging and WPA2-PSK security.
- **Scalability Considerations**: Designed to support future expansion of departments and devices.

## Network Design

- **Topology**: Star or hybrid star-bus configuration with centralized routing and switching.
- **Core Components**:
  - **2911 Router**: Inter-VLAN communication and external connectivity.
  - **2960 Switch**: VLAN and device interconnectivity.
  - **Access Points**: Wireless connectivity mapped to VLANs.
  - **DHCP Server**: Manages IP address allocation per VLAN.

## Configuration Details
1. **Routing**:
   - Static routing for efficient communication between VLANs.
   - NAT for secure internet access.
2. **Switching**:
   - VLANs for Admin, Finance, and Customer Service departments.
   - Layer 3 Switch Virtual Interfaces (SVIs) for inter-VLAN routing.
3. **IP Addressing**:
   - Admin/IT: 192.168.1.1/26
   - Finance/HR: 192.168.1.64/26
   - CS/Reception: 192.168.1.128/26
4. **Wireless Network**:
   - SSIDs: `Admin-WIFI`, `Finance-WIFI`, `CS-WIFI`
   - Security: WPA2-PSK authentication with unique passwords per VLAN.

## Testing and Validation
- **VLAN Connectivity**: Ping tests to verify device communication within VLANs.
- **Inter-VLAN Communication**: Ensures seamless routing between VLANs with access controls.
- **Wireless Functionality**: Validates connectivity and roaming across access points.
- **Performance Metrics**: Evaluated using latency, throughput, and DHCP lease verification.

## Results
- Successful deployment of a secure, scalable, and high-performance small office network.
- Improved traffic management and reduced congestion through VLAN segmentation.
- Reliable and secure communication between departments via inter-VLAN routing.

## Lessons Learned
- VLANs effectively enhance security and optimize network traffic.
- Importance of testing configurations in a simulation environment.
- Proper monitoring and documentation ensure efficient troubleshooting.
- 
## References
- [Cisco Documentation on VLANs and Inter-VLAN Routing](https://www.cisco.com/c/en/us/support/docs/lan-switching/inter-vlan-routing/41860-howto-L3-intervlanrouting.html)
- T. Lammle, *CCNA Routing and Switching Study Guide*, Sybex, 2016.
