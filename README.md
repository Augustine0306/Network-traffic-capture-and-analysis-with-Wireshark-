# Network-traffic-capture-and-analysis-with-Wireshark
## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.

### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).
## PROGRAM:
Wireshark Packet Capture and Filter Usage
## 1. Open Wireshark and Select a Network Interface

<img width="1909" height="1021" alt="Screenshot 2025-10-04 131921" src="https://github.com/user-attachments/assets/a033aa81-e727-4371-95c2-a027899514ce" />

## 2. Start Capturing Packets
• Click the blue shark fin icon or double-click the interface. • Wireshark will start capturing all real-time traffic.

<img width="954" height="1020" alt="Screenshot 2025-10-04 130629" src="https://github.com/user-attachments/assets/77040de1-6cda-4767-82c7-f326cfdb8110" />

## 3. Apply Filters to Focus on Specific Traffic
• Use filters like tcp.port == 80 in the top filter bar to narrow down results.
<img width="1919" height="744" alt="image" src="https://github.com/user-attachments/assets/69cbaff3-f511-4622-af67-ed65913ac35e" />


## 4. Analyze Packet Details
• Click on a packet to view its detailed breakdown including frame, Ethernet, IP, TCP/UDP layers, and data payload.

<img width="973" height="473" alt="Screenshot 2025-10-04 131647" src="https://github.com/user-attachments/assets/29d4d3ed-bdc5-484e-ac40-74ba9f1ad854" />

## 5.Analyse ip==10.82.65.160

<img width="1919" height="708" alt="image" src="https://github.com/user-attachments/assets/a7b0959b-5ee5-4f62-80d0-cd86cd6f3dd2" />


## 6.Analyse frames

<img width="1919" height="696" alt="image" src="https://github.com/user-attachments/assets/13ee4981-0642-4728-b841-2ef843c05118" />

## 7.Analyse tcp ports

<img width="1919" height="782" alt="image" src="https://github.com/user-attachments/assets/471c4f4e-4322-46b4-a0f0-9d91118c837f" />




## 5. Export or Save the Capture
• Go to File > Save As to store the capture in .pcap format for future analysis.

<img width="1919" height="1022" alt="Screenshot 2025-10-04 131741" src="https://github.com/user-attachments/assets/7a1af830-92fa-4a26-81c5-b5ae79434f62" />

## OUTPUT:
Captured Packets with Protocol Analysis and Detailed Packet Info

## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.
