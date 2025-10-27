# Cybersecurity-task-5

# Task 5 – Wireshark Network Traffic Analysis Report
**Name:** Muthukumaran R  
**Date:** (update date if required)  
**File Included:** `capture.pcap`

---

## 1) Environment Details
- **System:** macOS
- **Tool Used:** Wireshark
- **Interface Used:** Wi-Fi (en0)
- **Capture Duration:** ~60 seconds

---

## 2) Traffic Generation Performed During Capture
The following actions were executed to generate network traffic:

| Action | Performed |
|--------|------------|
| `ping -c 4 8.8.8.8` | Yes |
| `curl -I https://www.google.com` | Yes |
| `dig +short example.com` | Yes |
| Visited `https://example.com` | Yes |
| Visited `http://neverssl.com` | (Not Used / Optional) |

---

## 3) Protocols Identified in the Capture
At least four different network protocols were observed:

1. **DNS** – Name resolution for example.com and google.com  
2. **TLS (HTTPS)** – Encrypted web traffic from secure sites  
3. **HTTP** – Plain text traffic (if any unencrypted sites were opened)  
4. **ICMP** – Echo request/reply from `ping` command

---

## 4) Sample Packet Observations
- **DNS Packet**: Query request for `example.com` returned by resolver  
- **TLS Packet**: Client Hello observed during HTTPS session negotiation  
- **ICMP Packet**: Echo reply received from 8.8.8.8 with normal RTT  
- **HTTP Traffic**: Visible request headers under no-TLS environment (if captured)

---

## 5) Conclusion
The capture successfully demonstrated basic network communication behavior:
- DNS resolved domain names
- TLS secured HTTPS communication
- ICMP confirmed network reachability
- HTTP showed unencrypted requests if available

The `capture.pcap` file contains valid recorded traffic for educational and analysis purposes.

---

**Report Prepared By:**  
**Muthukumaran R**
