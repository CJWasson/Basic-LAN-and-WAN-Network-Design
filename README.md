# Basic LAN and WAN Network Design

This repository showcases my work in designing and implementing LAN and WAN networks. It includes step-by-step guides, configuration templates, and visual diagrams for various network setups, from home environments to small offices and multi-site WANs.

This repository provides comprehensive LAN and WAN network designs, including:

1. [Basic Home Network](docs/home-network.md)
2. [Small Office Network](docs/small-office-network.md)
3. [VLAN-Segmented Office/School Network](docs/vlan-network.md)
4. [Simple Wide Area Network (WAN)](docs/wan-network.md)

Each section includes components, network diagrams, implementation steps, and security tips.

---

## 🚀 How to Use
1. Explore the `docs/` folder for detailed guides.
2. View diagrams in the `visuals/` folder.
3. Access templates for network configuration in the `templates/` folder.

---

## 📚 Topics Covered
- Router and switch setup
- VLAN configuration
- IP addressing and DHCP
- Network security best practices

---

## 📁 Repository Structure
```
├── README.md         # Project overview and quick start
├── docs/             # Detailed network guides
│   ├── home-network.md
│   ├── small-office-network.md
│   ├── vlan-network.md
│   └── wan-network.md
├── templates/        # Configuration templates
│   ├── dhcp-config.txt
│   ├── vlan-config.txt
│   └── vpn-config.txt
├── visuals/          # Network diagrams
│   ├── home-network.png
│   ├── small-office-network.png
│   ├── vlan-network.png
│   └── wan-network.png
├── LICENSE           # License information
└── .gitignore        # Git ignore file
```

---

## 📄 Documentation

### **1. Basic Home Network**
**Purpose:** Establish a simple home network for internet access and device connectivity.

**Components:**
- Router (Gateway)
- Optional Switch (For wired connections)
- End Devices (PCs, smartphones, smart TVs)

**Network Design:**
```text
Internet --> Router --> Switch (Optional) --> End Devices (PCs, Printers)
                       --> Wi-Fi --> Wireless Devices (Smartphones, Laptops)
```

**Implementation Steps:**
1. Connect the router to the modem.
2. Access the router interface and configure the SSID and password.
3. Enable DHCP for automatic IP assignment.

**Security Tips:**
- Change the router's default admin credentials.
- Enable WPA3 encryption.
- Set up a guest network for visitors.

---

### **2. Small Office Network**
**Purpose:** Connect multiple office devices while ensuring security and organization.

**Components:**
- Router (Firewall and Gateway)
- Switch (For wired connections)
- Access Point (Wireless connectivity)
- End Devices (PCs, Laptops, Printers)

**Network Design:**
```text
Internet --> Router --> Switch --> End Devices (PCs, Printers)
                       --> Access Point --> Wireless Devices
```

**Implementation Steps:**
1. Connect the router to the modem and switch.
2. Assign static IPs for critical devices.
3. Enable the firewall and configure port forwarding if needed.

**Security Tips:**
- Enable MAC filtering.
- Separate guest and business networks.
- Install endpoint security software.

---

### **3. VLAN-Segmented Office/School Network**
**Purpose:** Segment network traffic into VLANs for better organization and security.

**Components:**
- Router (Firewall and Gateway)
- Managed Switch (Supports VLANs)
- Access Point (VLAN SSID support)
- End Devices (Desktops, Laptops, Printers)

**Network Design:**
```text
Internet --> Router --> Managed Switch --> VLANs:
                                   VLAN 10 (Staff) --> Staff Devices
                                   VLAN 20 (Students) --> Student Devices
                                   VLAN 30 (Guests) --> Guest Wi-Fi
                       --> Access Point --> VLAN SSIDs
```

**Implementation Steps:**
1. Configure VLANs on the managed switch.
2. Assign devices to VLANs based on roles.
3. Use ACLs to restrict cross-VLAN communication.

**Security Tips:**
- Enable VLAN tagging.
- Use port security.
- Monitor traffic for unusual patterns.

---

### **4. Simple Wide Area Network (WAN)**
**Purpose:** Connect multiple locations securely using a VPN.

**Components:**
- Routers (Branch and Main Office)
- VPN Tunnel (Encrypted communication)
- Firewall (Perimeter security)
- End Devices (PCs, Servers, Printers)

**Network Design:**
```text
Branch Office 1 --> VPN Tunnel --> Main Office --> VPN Tunnel --> Branch Office 2
                       |                                  |
                       End Devices                       End Devices
```

**Implementation Steps:**
1. Configure IPsec VPN tunnels.
2. Enable static or dynamic routing.
3. Set firewall rules to allow VPN traffic.

**Security Tips:**
- Use AES-256 encryption.
- Update router firmware regularly.
- Monitor VPN traffic for anomalies.

---

## 📜 License
This project is licensed under the [Restricted License](LICENSE).

## 🤝 Contributing
Feel free to submit pull requests or report issues.

## 📧 Contact
For questions, reach out via GitHub Issues or Discussions.
