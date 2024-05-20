# Wireshark-Project
Wireshark for Beginners: Capture Packets

## Objective
[Brief Objective - Remove this afterwards]

The Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned
[Bullet Points - Remove this afterwards]

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
[Bullet Points - Remove this afterwards]

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Task

## Task 1: Insatll Wireshark On Ubuntu




## Task 1 (Key Takeaways):
- The user can be added to the Wireshark group to add packet capture capabilities
- Wireshark should not be run as superuser for security reasons
- Latest softwear versions help ensure fewer technical mishaps or issues.
- To get latest stable verison of Wireshark use add-apt-repository command.
  
## Task 2: Start an packet capture on ethernet port and save it to file

## Step 2 (Key Takeaways):
- The wired interface includes controls to start packet cpature wich begind with 'en' in WireShark
- The Wireshark app includes controls to start packet capture, stop capture, save the packets to a file, and load the capture file.
- A capture can only be saved once the capture has stopped.

## Step 3: Use an Display filter to dettect Https packets

## Step 3 (Key Takeaways):
-To display certain packets in an existing packet capture, use a display filter.
-To display only HTTPS traffic, use a filter on TCP port 443: tcp.port == 443

## Task 4: Visit a webpage & dectect is ip address using a display filter

## Task 4 ( Key Takeaways):
-A TLS handshake display filter may be used to detect a website visit in a packet list: tls.handshake.type ==1A TLS handshake display filter may be used to detect a website visit in a packet list: tls.handshake.type ==1
-The IP address is used in a filter to obtain packet information for a particular website: ip.addr == 142.251.163.105

## Task 5: Locate all HTTPS packets froma a capture not containg an ip address

## Task 5 (Key Takeaways);
