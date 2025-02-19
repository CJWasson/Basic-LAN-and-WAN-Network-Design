# DHCP Configuration Template

This template provides the essential configuration settings for setting up a DHCP server.

---

## 📄 Example DHCP Configuration (Cisco IOS)
```shell
! Enable DHCP service
service dhcp

! Define DHCP pool for LAN
ip dhcp pool LAN_POOL
 network 192.168.10.0 255.255.255.0
 default-router 192.168.10.1
 dns-server 8.8.8.8 8.8.4.4
 lease 7

! Exclude static IPs from the pool
ip dhcp excluded-address 192.168.10.1 192.168.10.20
```

---

## ⚙️ Key Configuration Parameters
- **Network:** Defines the subnet for DHCP clients.
- **Default Router:** Specifies the gateway for client devices.
- **DNS Server:** Provides DNS resolution for clients.
- **Lease:** Duration for which IP addresses are assigned.
- **Excluded Addresses:** Prevents DHCP from assigning static IPs.

---

## 🔧 Verification Commands
Run the following commands to verify DHCP status:
```shell
show ip dhcp pool
show ip dhcp binding
show ip dhcp conflict
```

---

## 🛠️ Troubleshooting Tips
- Ensure the DHCP service is enabled.
- Check for IP conflicts in the binding table.
- Verify excluded addresses to avoid assignment overlap.

---

This configuration ensures efficient IP management and prevents conflicts in the network.
