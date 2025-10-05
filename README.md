# Task-8

# 🧩 VPN Usage & Security Audit  

---

## 🧠 Objective
To evaluate the functionality, privacy protection, and performance impact of a reputable free VPN service.  
The audit includes installation, connection testing, IP verification, encryption validation, and performance comparison.

---

## 🧰 Tools & Environment
- **VPN Chosen:** Proton VPN (Free Plan)  
- **Operating System:** Windows 11  
- **Browser:** Google Chrome (latest version)  
- **Test Websites:**  
  - [https://whatismyipaddress.com](https://whatismyipaddress.com) – IP verification  
  - [https://ipleak.net](https://ipleak.net) – DNS leak test  
  - [https://www.speedtest.net](https://www.speedtest.net) – Speed benchmarking  

---

## 🪜 Steps Performed

### 1️⃣ Choose and Install VPN
- Selected **Proton VPN (Free)** for its reputation, no-data-cap policy, and strong encryption.
- Created a free account and installed the Proton VPN desktop client from the official website.
- Logged in securely using provided credentials.

### 2️⃣ Connect to a VPN Server
- Chose **Netherlands** as the server location (closest available for optimal performance).  
- Established a successful connection confirmed via the Proton VPN interface.

### 3️⃣ Verify IP Address Change
- Checked public IP using **whatismyipaddress.com** before and after connection.  
- Observed that the IP changed from a local ISP IP (redacted for privacy) to a VPN-assigned IP in the Netherlands.  
- This confirmed traffic was being routed through the VPN server.

### 4️⃣ Confirm Encrypted Traffic
- Accessed several HTTPS websites to ensure data transmission remained secure.  
- Verified VPN tunnel encryption (AES-256) using Proton’s documentation.  
- Performed a DNS leak test at **ipleak.net** — no DNS leaks detected.

### 5️⃣ Measure Performance
- Ran a speed test before and after connecting to the VPN:

| Test Condition | Download Speed | Upload Speed | Ping |
|----------------|----------------|---------------|------|
| Before VPN | ~80 Mbps | ~25 Mbps | 20 ms |
| After VPN | ~55 Mbps | ~18 Mbps | 30 ms |

- **Result:** ~30% drop in speed, which is expected due to encryption overhead and distance to the server.

### 6️⃣ Disconnect and Compare
- Disconnected from the VPN and verified that the IP reverted to the original ISP IP.  
- Browsing speed and latency returned to normal levels.

---

## 🔐 Research on VPN Security

### **Encryption**
- Proton VPN uses **AES-256** encryption with **OpenVPN** and **WireGuard** protocols.  
- Encryption ensures all data packets are unreadable to ISPs, hackers, or network eavesdroppers.

### **Privacy Protection**
- VPN hides your **IP address** and masks your location.  
- Prevents websites and ISPs from tracking online activities.  
- Provides safer access when using public Wi-Fi networks.

### **Common Risks of Free VPNs**
- Some free VPNs may log data or inject ads.  
- Limited server choices and slower speeds.  
- Possible data caps and lack of support for torrenting or streaming.  
- Always verify the VPN provider’s **privacy policy** and **jurisdiction**.

---

## ⚖️ Benefits vs Limitations

| **Benefits** | **Limitations** |
|---------------|-----------------|
| Protects data with strong encryption | May reduce internet speed |
| Masks real IP & location | Limited server options on free plans |
| Bypasses geo-blocks | Some free VPNs log user data |
| Secures public Wi-Fi usage | Not a substitute for antivirus/firewall |
| Enhances privacy online | May not work with some restricted services |

---

## 📋 Conclusion
Proton VPN’s free plan effectively:
- Changed the public IP address  
- Encrypted web traffic  
- Prevented DNS leaks  
- Maintained reasonable performance  

This demonstrates that even a reputable free VPN can provide solid privacy protection for general use.  
However, users should be aware of **speed trade-offs** and **limitations of free tiers**.

---

## 🛡 Privacy & Safety Notes
- All real IPs and personal data are **redacted for privacy**.  
- No screenshots or logs containing sensitive information are included in this repository.  
- The purpose of this documentation is educational and non-commercial.

---

## 🧾 Repository Contents
vpn-audit/
├─ README.md # This file
├─ before_ip.txt # Contains “Redacted for privacy”
├─ after_ip.txt # Contains “Redacted for privacy”
├─ speed_before.txt # Contains recorded speed test summary
├─ speed_after.txt # Contains recorded speed test summary
└─ .gitignore # Ignores sensitive or system files

## 📚 References
- [Proton VPN Official Website](https://protonvpn.com)  
- [WhatIsMyIPAddress.com](https://whatismyipaddress.com)  
- [IPLeak.net DNS Leak Test](https://ipleak.net)  
- [Speedtest.net by Ookla](https://www.speedtest.net)  
- [Mozilla: How VPNs Work](https://www.mozilla.org/en-US/products/vpn/learn/how-do-vpns-work/)  

---

**End of Report**
