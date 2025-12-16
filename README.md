# Zero-Trust Network Segmentation Lab

This lab demonstrates how to design and implement a micro‑segmented network following zero‑trust principles.

- **Plan the segmentation:** Identify critical assets and users, then design separate network zones (user, server and management). Document your segmentation plan and create a network diagram.
- **Deploy the firewall:** Install pfSense or OPNsense on a VM or physical device. Create VLANs or subnets for each zone and assign interfaces accordingly.
- **Implement least‑privilege rules:** Configure firewall policies to allow only necessary traffic between zones (for example, user zone to server zone via specific ports). Block all other traffic by default.
- **Enable identity‑based access:** Integrate the firewall with an identity provider (e.g., LDAP, RADIUS) so that access decisions can be based on user identity and device posture.
- **Test and validate:** Generate test traffic between zones to verify that unauthorized lateral movement is blocked and legitimate traffic flows as intended. Use tools like nmap or ping to test connectivity.
- **Monitor and refine:** Collect firewall logs and flow data in your SIEM. Adjust rules and policies to improve security and performance.

All steps rely on open‑source software and publicly available documentation. This repository contains the lab guide and documentation to build your own zero‑trust segmentation environment.
