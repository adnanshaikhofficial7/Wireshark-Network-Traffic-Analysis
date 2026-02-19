📡 Task 5 – Network Traffic Capture and Analysis Using Wireshark
📌 Objective

The objective of this task was to capture live network traffic using Wireshark and analyze different network protocols including HTTP, TCP, and DNS. 
The goal was to understand how network communication occurs across different layers of the OSI model.



🛠️ Tools Used

Wireshark
Windows 10
Ethernet Network Interface


📂 Capture Details

Interface Used: Ethernet 3
Total Packets Captured: 22,953+
Capture File: task5_full_capture.pcap


🌐 Protocol Analysis

1️⃣ HTTP Analysis

Source IP: 192.168.84.7
Destination IP: 184.27.197.88
Source Port: 1140
Destination Port: 80
Protocol: HTTP
Method: GET
Requested Resource: /msdownload/update/others/2026/02/44767133_47b174242a39f3fdfe1e6f8c50efacad599014d.cab

📖 Explanation:
This packet shows an HTTP GET request from the client system requesting a Windows update CAB file from a web server using TCP port 80.

2️⃣ TCP Analysis (HTTPS Communication)

Source IP: 192.168.84.7
Destination IP: 34.104.35.123
Source Port: 1036
Destination Port: 443
Protocol: TCP
Packet Length: 54 bytes

📖 Explanation:
This packet represents TCP communication over port 443 (HTTPS). It shows acknowledgment packets involved in secure web communication.

3️⃣ DNS Analysis

Source IP: 192.168.84.7
Destination IP: 192.168.84.94
Transport Protocol: UDP
Destination Port: 53
Query: beacons.gcp.gvt2.com

📖 Explanation:
This DNS query shows the client resolving a domain name to its corresponding IP address before establishing a connection.

🖼️ Screenshots Included

HTTP Packet Analysis
DNS Query Analysis
TCP Packet Analysis
Full Traffic Capture

🎯 Key Observations

HTTP traffic uses TCP port 80.
HTTPS communication uses TCP port 443.
DNS queries use UDP port 53.
Network communication follows layered architecture (OSI model).
Domain name resolution occurs before HTTP/HTTPS communication.

🏁 Conclusion

This task successfully demonstrated real-time network traffic capture and protocol analysis using Wireshark. 
Multiple protocols were identified and analyzed at different OSI layers. 
The exercise improved understanding of packet structure, TCP/IP communication, DNS resolution, and HTTP request handling.
