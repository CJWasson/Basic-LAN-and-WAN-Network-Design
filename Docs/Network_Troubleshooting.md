# Network Troubleshooting Guide

This guide provides step-by-step instructions for diagnosing and resolving common network issues in LAN and WAN environments.

---

## 🔍 Overview
Efficient troubleshooting requires a systematic approach. This guide covers common issues, diagnostic tools, and solutions for network problems.

This guide covers the following:
1. Common Network Issues
2. Troubleshooting Steps
3. Useful Tools
4. Preventive Measures

---

## ⚠️ 1. Common Network Issues

| Issue                     | Symptoms                                      | Possible Causes                   |
|---------------------------|-----------------------------------------------|-----------------------------------|
| No Internet Connection    | Cannot browse, ping, or access external sites  | ISP issues, router failure, DNS   |
| Slow Network Performance | High latency, buffering, slow downloads         | Bandwidth congestion, interference|
| IP Address Conflicts      | Devices unable to connect                      | Duplicate IP assignment           |
| Intermittent Connectivity | Devices drop connection periodically           | Weak signal, firmware bugs        |
| VLAN Communication Issues | Devices in different VLANs cannot communicate  | Misconfigured VLAN or ACL         |

---

## 🛠️ 2. Troubleshooting Steps
1. **Check Physical Connections:**
   - Verify cables are properly connected and not damaged.
   - Ensure devices are powered on and indicator lights are active.

2. **Verify IP Configuration:**
   - Run `ipconfig` (Windows) or `ifconfig` (Linux/Mac) to check IP addresses.
   - Ensure devices are on the correct subnet.

3. **Test Connectivity:**
   - Use `ping` to test connectivity to the gateway and external sites.
   - Use `traceroute` to identify where packets are dropping.

4. **Check DNS Resolution:**
   - Test DNS using `nslookup` or `dig`.
   - Change DNS servers if resolution fails (e.g., Google DNS `8.8.8.8`).

5. **Review Router and Switch Configuration:**
   - Verify DHCP settings and address pool.
   - Check VLAN and port assignments on the switch.

6. **Inspect Firewall Rules:**
   - Ensure traffic is not being blocked between devices.

7. **Monitor Traffic:**
   - Use `Wireshark` or `tcpdump` to capture and analyze network traffic.

8. **Check for Firmware Updates:**
   - Update router, switch, and access point firmware to fix known bugs.

---

## 🔧 3. Useful Tools
- **Ping:** Tests connectivity to other devices.
- **Tracert/Traceroute:** Shows the path packets take to reach the destination.
- **Nslookup/Dig:** Tests DNS resolution.
- **Wireshark:** Captures and analyzes network traffic.
- **IP Scanner:** Identifies active devices on the network.

---

## 🔒 4. Preventive Measures
- **Network Monitoring:** Use SNMP, PRTG, or Nagios for real-time alerts.
- **Configuration Backups:** Regularly back up router and switch configurations.
- **Firmware Updates:** Keep all network devices updated.
- **IP Address Management:** Avoid conflicts by assigning static IPs for critical devices.
- **VLAN Segmentation:** Isolate traffic to prevent broadcast storms.

---

## 📄 Documentation and Logs
- Document network topology, IP ranges, and VLAN assignments.
- Maintain logs of network issues and resolutions for future reference.

This troubleshooting approach ensures faster resolution of network problems and helps maintain a stable, efficient network environment.
