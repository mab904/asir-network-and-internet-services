# 🖧 Network and Internet Services – ASIR Module

This repository contains the practical assignments from the Security and High Availability module. 
(Most of the documents are hands‑on labs focused on basic Linux network services such as mail servers, Apache, FTP, DNS and DHCP.)  
The documentation is in Spanish and organized by topics to make navigation easier. If you need any clarification, I’ll be happy to help 😁. (The practices are documented through PDF files containing screenshots and explanations)

## Contents

### UT1 – DHCP
The first practice focuses on deploying a standard DHCP server, understanding how scopes, leases, and option fields are defined, and observing how clients obtain their network settings dynamically. The second practice extends these concepts to more advanced scenarios, implementing DHCP in Linux with a failover configuration to ensure service continuity and high availability. It also incorporates the use of a relay agent to forward DHCP requests across different network segments.

### UT2 – DNS
Domain Name System provides naming, resolution, and delegation services across IP networks. The first practice focuses on deploying a functional DNS server, defining zones, resource records, and forward/reverse lookups to understand how human‑readable names are translated into network addresses. The second practice extends these foundations by implementing a master–slave architecture, introducing zone transfers, serial management, and redundancy mechanisms that ensure consistency and availability across DNS servers.

### UT3 – FTP Service and Secure File Transfer (This one is very interesting 👌)
This practices focus on deploying a FTP service using VSFTPD within a functional domain and DNS environment. The practice includes enabling anonymous access, configuring passive mode, creating virtual users independent from system accounts, securing communication with SSL, and testing all functionalities using FileZilla as the FTP client.

### UT4 – Web (Apache 🦝)
Apache as a web server. The first practice covers the installation of Apache, enabling PHP modules, hosting a PHP‑based quiz application, and creating multiple virtual hosts both by name and by port, including public sites and restricted private sites with custom error pages. The second practice extends the setup by enabling SSL/TLS certificates for secure HTTPS access and configuring Apache server‑status to monitor real‑time activity such as connected clients, CPU load, uptime, and requested resources.

### UT5 – Email Service
Deploying and testing a complete email service using Postfix. The practice begins with the local configuration of a Postfix mail server, allowing users from the same domain to exchange messages internally. It then expands to a multi‑server setup by configuring two separate domains on different Postfix servers, enabling cross‑domain communication. The configuration is verified through Telnet SMTP tests and by sending messages between domains using the mailx client. Finally, the unit includes setting up Thunderbird to access and read mail from one server.

### UT6 – Streaming (I didn’t expect this practice to be so easy to carry out.)
Implementing HLS (HTTP Live Streaming) using Nginx with the RTMP module and FFmpeg. The practice consists of configuring Nginx to receive a video stream and generate HLS segments, sending a live video feed from FFmpeg to the server, and testing playback through an HTML5 video player in a web browser. The setup includes enabling RTMP input, generating .m3u8 playlists and video fragments, and serving them over HTTP so clients can reproduce the stream in real time.
