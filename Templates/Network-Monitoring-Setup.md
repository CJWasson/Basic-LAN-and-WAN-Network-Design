# Network Monitoring Setup

This template provides the essential configuration steps for setting up network monitoring using SNMP, PRTG, or Nagios.

---

## 📡 1. Enable SNMP on Network Devices

### Example SNMP Configuration (Cisco IOS)
```shell
snmp-server community PUBLIC RO
snmp-server community PRIVATE RW
snmp-server location Main_Office
snmp-server contact admin@yourdomain.com
```

**Key Parameters:**
- **Community Strings:** `PUBLIC` (read-only) and `PRIVATE` (read-write).
- **Location:** Identifies device location.
- **Contact:** Admin email for notifications.

---

## 🖥️ 2. PRTG Monitoring Setup

1. **Install PRTG:** Download from [Paessler's website](https://www.paessler.com/prtg) and install on a monitoring server.
2. **Add Devices:**
   - Navigate to *Devices > Add Device*.
   - Enter the IP address and SNMP credentials.
3. **Add Sensors:**
   - Use *SNMP Traffic*, *Ping*, and *CPU Load* sensors.
4. **Set Alerts:**
   - Create thresholds for high bandwidth or device failures.

---

## 📊 3. Monitor and Analyze
- **PRTG Dashboard:** Real-time graphs and alerts.
- **Nagios Web Interface:** Detailed status and logs.
- **SNMP Polling:** Collect traffic, CPU, and memory data.

---

## 🛠️ 5. Troubleshooting Tips
- Ensure SNMP is enabled on all devices.
- Check firewall rules for SNMP (UDP port 161).
- Verify community strings match in monitoring tools.
- Monitor log files for errors (`/var/log/nagios/`).

---

This setup ensures proactive network monitoring and quick identification of performance issues.

