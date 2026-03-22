# Network Traffic Analysis using Kali Linux

## 📌 Project Objective
The objective of this project is to capture and analyze network traffic to identify normal and suspicious patterns using Wireshark, tcpdump, and Snort.

---

## 🛠 Tools Used
- Kali Linux
- Wireshark
- tcpdump
- Snort

---

## 📂 Project Structure
Network-Traffic-Analysis/
│── capture.pcap
│── Screenshots/
│── Documentation.pdf
│── README.md

---

## 🚀 Methodology

### 1. Capturing Live Traffic
Live network traffic was captured using Wireshark from the active network interface.

### 2. Traffic Generation
The following activities were performed:
- Ping requests to google.com
- Browsing websites
- DNS lookup
- Port scanning using Nmap

### 3. Traffic Analysis

#### ICMP Analysis
Filter used:
icmp

Observed echo request and reply packets.

#### DNS Analysis
Filter used:
dns

Observed domain name resolution queries.

#### HTTP Analysis
Filter used:
http

Observed HTTP GET requests.

#### SYN Scan Detection
Filter used:
tcp.flags.syn == 1 && tcp.flags.ack == 0

Detected multiple SYN packets indicating port scan activity.

---

## 🔍 Findings

- DNS queries were observed for domain resolution.
- TCP 3-way handshake was identified.
- Port scan activity was detected using SYN packet patterns.
- HTTP communication was visible in plaintext.

---

## 📌 Conclusion
Network traffic analysis helps detect suspicious activities such as port scanning and abnormal traffic patterns. Tools like Wireshark and Snort are effective for intrusion detection and monitoring.

---

## 📎 Author
Tejas Agarwal
Cybersecurity Intern
