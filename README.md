# Wireshark Project
Wireshark for Beginners: Capture Packets

## Objective
The Wireshark project aimed to establish a controlled environment for capturing and analyzing network traffic. The primary focus was on using Wireshark to gain hands-on experience in network security, understanding protocols, and detecting network issues and attacks.

### Skills Learned

- Understanding SIEM concepts and practical application.
- Analyzing and interpreting network logs.
- Generating and recognizing attack signatures and patterns.
- Knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Task

### Task 1: Install Wireshark on Ubuntu
- **Key Takeaways**:
  - Users can be added to the Wireshark group to enable packet capture capabilities.
  - Wireshark should not be run as superuser for security reasons.
  - Using the latest software versions helps ensure fewer technical issues.
  - To get the latest stable version of Wireshark, use the `add-apt-repository` command.

### Task 2: Start a Packet Capture on Ethernet Port and Save it to File
- **Key Takeaways**:
  - The wired interface, usually starting with 'en', is used for packet capture in Wireshark.
  - Wireshark includes controls to start, stop, save packet captures, and load capture files.
  - A capture can only be saved once it has stopped.

### Task 3: Use a Display Filter to Detect HTTPS Packets
- **Key Takeaways**:
  - To display certain packets in an existing capture, use a display filter.
  - To display only HTTPS traffic, use a filter on TCP port 443: `tcp.port == 443`.

### Task 4: Visit a Webpage & Detect its IP Address Using a Display Filter
- **Key Takeaways**:
  - A TLS handshake display filter can be used to detect a website visit in a packet list: `tls.handshake.type == 1`.
  - Use the IP address in a filter to obtain packet information for a specific website: `ip.addr == 142.251.163.105`.

### Task 5: Locate All HTTPS Packets from a Capture Not Containing an IP Address
- **Key Takeaways**:
  - Display filters can be used to exclude certain IP addresses from the capture.
  - To locate HTTPS packets that do not contain a specific IP address, use a filter to exclude that address: `ip.addr != 142.251.163.105`.
  - Understanding how to filter out specific IP addresses is useful for focusing on relevant traffic and reducing noise in the data.
