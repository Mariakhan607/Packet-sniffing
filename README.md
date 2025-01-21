# Packet-sniffing
Project Report on Packet Sniffing Using Wireshark
Introduction
In an era where data breaches and cyber threats are increasingly prevalent, understanding the vulnerabilities associated with data transmission is crucial. Packet sniffing is a technique used to intercept and log traffic that passes over a digital network. This project aims to illustrate how unencrypted data, such as user credentials, can be captured during transmission.

Packet Sniffing
Packet sniffing refers to the process of capturing data packets that travel across a network. This technique can be used for various purposes, including network troubleshooting, performance monitoring, and security analysis. However, it can also be exploited by malicious actors to intercept sensitive information, such as usernames and passwords, if the data is not adequately protected.

Wireshark
Wireshark is an open-source network protocol analyzer that allows users to capture and interactively browse the traffic running on a computer network. It provides a comprehensive view of the data packets, including their source, destination, and content. Wireshark supports a wide range of protocols and is widely used in both academic and professional settings for network analysis and security assessments.

Methodology
The project was conducted in a controlled environment to ensure ethical standards were maintained. The following steps outline the methodology used in this project:

Environment Setup:

Operating System: Windows 10
Wireshark Version: 3.6.0
Network Configuration: A local network was established with a test machine running the Acunetix web application.
Packet Capture:

Launching Wireshark: Wireshark was launched, and the appropriate network interface was selected for packet capture.
Starting Capture: The packet capture process was initiated, allowing Wireshark to log all network traffic.
Interacting with Acunetix: A test user account was created on the Acunetix web application, and the login process was executed to generate traffic containing credentials.
Data Analysis:

Filtering Traffic: Wireshark's filtering capabilities were used to isolate HTTP packets, as the login credentials were transmitted over this protocol.
Inspecting Packets: The relevant packets were examined to extract the HTTP POST request containing the login credentials.
Results
The analysis revealed that the login credentials (username and password) were transmitted in plaintext within the HTTP POST request. The captured packet data included:

Source IP: [User 's IP Address]
Destination IP: [Acunetix Server IP Address]
HTTP Method: POST
Request Body: username=exampleUser &password=examplePassword
Conclusion
This project successfully demonstrated the vulnerabilities associated with unencrypted data transmission. The use of Wireshark allowed for the effective capture and analysis of network traffic, revealing sensitive information that could be exploited by malicious actors. It is imperative for organizations to implement secure protocols, such as HTTPS, to protect user credentials and sensitive data during transmission.

Recommendations
Use Encrypted Protocols: Always use HTTPS instead of HTTP to encrypt data in transit.
Network Security Measures: Implement firewalls and intrusion detection systems to monitor and protect network traffic.
User Education: Educate users about the importance of secure passwords and recognizing phishing attempts.
References
Wireshark Official Documentation: Wireshark
Acunetix Official Website: Acunetix
