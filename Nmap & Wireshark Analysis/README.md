# Network Analysis Using Nmap & Wireshark

This project involved active network scanning using Nmap and packet capture analysis using Wireshark to assess host visibility, detect anomalies, and recommend mitigation strategies.

## 🔧 Tools Used
- Nmap (port scanning and host identification)
- Wireshark (packet inspection and traffic analysis)
- Zenmap (topology visualization)
- NetworkMiner (connection metadata)
- CIS Controls & NIST SP 800-53 as mitigation frameworks

## 📊 Key Findings
- Identified 6 active hosts on the 10.168.27.0/24 subnet, including Windows and Linux machines
- Exposed ports included LDAP, SMB, FTP, and SSH—some representing legacy risks
- Detected potential port scanning activity from external host 10.16.80.243
- Observed high-frequency RST/FIN TCP flags indicating half-open connections and scan attempts

## 🛡️ Recommendations
- Apply security patches to LDAP/SMB services and replace FTP with SFTP
- Disable legacy ports (e.g., echo, chargen) and enforce secure SSH configurations
- Deploy IDS/IPS (e.g., Snort or Suricata) with rules to detect port scanning
- Implement firewall rules and network segmentation to limit exposure

## 📄 Deliverables
- PDF report of scan results and analysis
- Screenshots of Zenmap topology and Wireshark flags
- Reference to industry frameworks and vendor best practices

## ⚠️ Disclaimer
This project was developed as part of academic cybersecurity coursework. All data and systems were simulated in a lab environment for educational purposes only.
