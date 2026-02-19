# WireShark_Task_5_Elevate-Labs

Wireshark is a free, open-source network protocol analyzer that captures and inspects data packets traveling over a network. It's widely used by network administrators, security professionals, and developers to troubleshoot issues, analyze performance, and detect anomalies. It supports hundreds of protocols and provides detailed packet-level insights.

*Capturing Network Traffic*

Select Interface: Launch Wireshark. In the main window, choose a network interface (e.g., Ethernet, Wi-Fi) from the list. Click the shark fin icon (or "Start") to begin capturing.
Apply Filters (Optional): Before starting, set a capture filter in the "Capture Options" dialog (e.g., "host 192.168.1.1" to capture traffic to/from a specific IP).
Start Capture: Click "Start." Wireshark will display packets in real-time as they flow.
Stop Capture: Click the red square icon when done. Save the capture file (.pcapng) for later analysis.

Tips:

Use promiscuous mode (enabled by default) to capture all packets on the network segment.
For wireless, ensure your adapter supports monitor mode.
Avoid capturing on public Wi-Fi without consent.
Analyzing Captured Traffic
Load Capture: Open a saved .pcapng file or use the live capture.
Display Filters: Use the filter bar at the top to narrow down packets (e.g., "tcp.port == 80" for HTTP traffic, "ip.src == 10.0.0.1" for source IP).
Inspect Packets: Click a packet in the list to view details in the middle pane (packet dissection) and raw data in the bottom pane (hex dump).

*Key Analysis Features:*

Statistics: Go to "Statistics" menu for summaries like protocol hierarchy, conversations, or endpoints.
Follow Streams: Right-click a packet and select "Follow > TCP Stream" to reconstruct data flows (e.g., view HTTP requests/responses).
Expert Info: Check the "Expert Info" window for warnings/errors (e.g., retransmissions indicating network issues).
Color Coding: Wireshark colors packets by type (e.g., green for TCP, blue for UDP) for quick visual scanning.
Export Data: Save filtered results or export to CSV/JSON for further processing.
Common Use Cases:

Troubleshooting: Identify latency by checking packet timestamps and flags.
Security: Detect anomalies like unusual ports or encrypted traffic patterns.
Performance: Analyze bandwidth usage with IO graphs (under Statistics).
