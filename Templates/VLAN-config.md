# VLAN Configuration Template

This template provides the essential configuration settings for creating and managing VLANs on a managed switch.

---

## 📄 Example VLAN Configuration (Cisco IOS)
```shell
Create VLANs
vlan 10
 name STAFF
vlan 20
 name STUDENTS
vlan 30
 name GUESTS

Assign VLANs to switch ports
interface range GigabitEthernet0/1-5
 switchport mode access
 switchport access vlan 10

interface range GigabitEthernet0/6-10
 switchport mode access
 switchport access vlan 20

interface GigabitEthernet0/11
 switchport mode access
 switchport access vlan 30

Configure Trunk Port (for inter-VLAN communication)
interface GigabitEthernet0/24
 switchport mode trunk
 switchport trunk allowed vlan 10,20,30
```

---

## ⚙️ Key Configuration Parameters
- **VLAN IDs:** Unique identifiers for each VLAN (e.g., 10, 20, 30).
- **VLAN Names:** Descriptive names for each VLAN (e.g., STAFF, STUDENTS, GUESTS).
- **Access Ports:** Assign end devices to specific VLANs.
- **Trunk Ports:** Allow traffic from multiple VLANs across switches.

---

## 🔧 Verification Commands
Run the following commands to verify VLAN configuration:
```shell
show vlan brief
show interfaces switchport
show running-config
```

---

## 🛠️ Troubleshooting Tips
- Ensure all VLANs are created and active.
- Verify trunk ports allow required VLANs.
- Check port mode (access vs. trunk).
- Confirm end devices receive correct IP addresses.

---

This configuration ensures proper traffic segmentation, enhancing network security and performance.
