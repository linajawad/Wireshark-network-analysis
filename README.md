# Wireshark-network-analysis
Basic packets capture and analysis using Wireshark

## Overview
This project demonstrates basic network packet capture and analysis using Wireshark, a powerful open-source protocol analyzer. The goal is to observe network traffic, identify common protocols, and analyze patterns or anomalies based on real-time capture.

## Objectives
- Learn how to capture live network traffic using Wireshark.
- Identify and filter various protocols (e.g., TCP, UDP, HTTP, DNS).
- Compare results between different types of traffic (e.g., normal browsing vs. video streaming).
- Gain hands-on experience in network troubleshooting and security awareness.

## Tools Used
- Wireshark (Version X.X)
- Operating System: Windows 10 / Linux / macOS (choose the one you used)
- Sample `.pcapng` files for offline analysis

## Capture Scenarios
| Scenario                 | Description                            | Protocols Observed       |
|--------------------------|----------------------------------------|---------------------------|
| Normal web browsing      | Visiting websites (HTTP/HTTPS)         | HTTP, TCP, DNS, TLS       |
| Video streaming (YouTube)| Watching videos                        | TCP, QUIC, TLS, UDP       |
| DNS resolution           | Resolving domain names manually        | DNS, UDP                  |

## Key Findings
- Web traffic (HTTPS) is encrypted using TLS, preventing detailed content inspection.
- Video streaming generates high-volume traffic and often uses QUIC/UDP instead of traditional TCP.
- DNS queries are lightweight but frequent; they can reveal visited domains if not encrypted.

## Screenshots
Include screenshots of Wireshark filters, packet details, and graphs (optional).

## How to Run
1. Install Wireshark from [https://www.wireshark.org/](https://www.wireshark.org/).
2. Open a `.pcap` file included in this repo (if available) or capture your own.
3. Apply filters like:
   - `http`
   - `tcp.port == 443`
   - `dns`
4. Analyze the packet details, info columns, and use Statistics > Protocol Hierarchy.

## Conclusion
This analysis gives practical exposure to network packet structures and helps understand how different protocols behave on a real network. Wireshark is a key tool for network administrators, cybersecurity students, and IT professionals.

---

## Author
Lina Jawad - CyberSecurity Student
