# Simple WAN Network Guide

This guide provides step-by-step instructions for setting up a secure Wide Area Network (WAN) to connect multiple office locations.

---

## 🌐 Overview
A WAN connects remote sites, allowing devices in different locations to communicate securely. This guide focuses on using VPN tunnels to protect data across the internet.

This guide covers the following:
1. Network Components
2. WAN Configuration Steps
3. Security Best Practices
4. Troubleshooting Tips

---

## 🛠️ 1. Network Components
- **Router:** At each location, configured for VPN.
- **Firewall:** To secure each network.
- **VPN Tunnel:** Encrypts communication between sites.
- **End Devices:** PCs, servers, and printers at each site.

**Network Design:**
```text
Branch Office 1 --> VPN Tunnel --> Main Office --> VPN Tunnel --> Branch Office 2
                       |                                  |
                       End Devices                       End Devices
```

---

## 🔧 2. WAN Configuration Steps
1. **Router Configuration:**
   - Set up VPN tunnels using IPsec.
   - Assign static IPs for routers at each site.

2. **VPN Setup:**
   - Use AES-256 encryption for secure tunnels.
   - Enable Dead Peer Detection (DPD) to monitor tunnel health.

3. **Routing Configuration:**
   - Enable static or dynamic routing (e.g., OSPF) between sites.

4. **Firewall Configuration:**
   - Allow VPN traffic (UDP ports 500 and 4500).

5. **IP Addressing:**
   - Ensure each site has a unique subnet (e.g., `192.168.10.0/24` for Site 1, `192.168.20.0/24` for Site 2).

---

## 🔒 3. Security Best Practices
- **Strong Encryption:** Use AES-256 for VPN tunnels.
- **VPN Authentication:** Use pre-shared keys or certificates.
- **Access Control:** Restrict access between sites as needed.
- **Firmware Updates:** Keep routers and firewalls up to date.
- **Monitoring:** Enable logging for VPN tunnel activity.

---

## 🛠️ 4. Troubleshooting Tips
- **VPN Tunnel Down:** Verify IPsec settings and pre-shared keys.
- **No Cross-Site Communication:** Check routing tables and firewall rules.
- **Slow Performance:** Ensure the WAN link has sufficient bandwidth.
- **IP Conflicts:** Ensure unique subnets for each site.

---

## 📄 Documentation and Backups
- Document VPN settings, IP addresses, and routing configurations.
- Back up router and firewall configurations regularly.

This setup ensures secure, reliable communication between multiple office locations over the internet.
