# VPN Configuration Template

This template provides the essential configuration settings for setting up an IPsec site-to-site VPN tunnel between two locations.

---

## 📄 Example VPN Configuration (Cisco IOS)
```shell
crypto isakmp policy 10
 encryption aes 256
 hash sha256
 authentication pre-share
 group 14
 lifetime 86400

crypto isakmp key VPN_SHARED_KEY address 203.0.113.2

crypto ipsec transform-set VPN_TRANSFORM_SET esp-aes 256 esp-sha256-hmac

crypto map VPN_MAP 10 ipsec-isakmp
 set peer 203.0.113.2
 set transform-set VPN_TRANSFORM_SET
 match address VPN_TRAFFIC

interface GigabitEthernet0/0
 crypto map VPN_MAP

ip access-list extended VPN_TRAFFIC
 permit ip 192.168.10.0 0.0.0.255 192.168.20.0 0.0.0.255

route-map VPN_ROUTE permit 10
 match ip address VPN_TRAFFIC
 set peer 203.0.113.2
```

---

## ⚙️ Key Configuration Parameters
- **Encryption:** AES-256 for data encryption.
- **Hashing:** SHA-256 for data integrity.
- **Pre-shared Key:** Used for VPN peer authentication.
- **Transform Set:** Defines IPsec encryption and hashing algorithms.
- **Access List:** Identifies traffic to encrypt.

---

## 🔧 Verification Commands
Run the following commands to verify VPN tunnel status:
```shell
show crypto isakmp sa
show crypto ipsec sa
show crypto map
```

---

## 🛠️ Troubleshooting Tips
- Ensure pre-shared keys match on both sides.
- Verify IP addressing and subnet settings.
- Check firewall rules for UDP ports 500 and 4500.
- Confirm ISAKMP and IPsec policies align between peers.

---

This configuration ensures secure site-to-site communication over the internet.
