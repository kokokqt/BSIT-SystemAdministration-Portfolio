Week 2 Portfolio Project — Enterprise Infrastructure Planning for a Startup Company

Course: ITEP 414 – System Administration and Maintenance Program: Bachelor of Science in Information Technology Project Type: Individual Portfolio Project Student: Villanueva, Mel Andrei A.

 Project Overview

Every successful IT infrastructure begins with proper planning. This project puts me in the role of a Junior System Administrator tasked with preparing the complete IT Infrastructure Plan for Vantix Technologies, a newly established software development company with 20 employees and zero existing infrastructure — no computers, no server, no network, no internet, and no security policies.

The final deliverable is a professional Enterprise Infrastructure Plan — the kind of document that could realistically be submitted to an IT Manager or Company Executive before any equipment is purchased.

 Learning Objectives
Explain the roles and responsibilities of a System Administrator
Identify the hardware, software, and networking requirements of a small business
Describe the purpose of IT documentation and infrastructure planning
Analyze organizational IT requirements
Prepare professional IT inventories
Design an enterprise network topology
Create technical documentation using Markdown
Present infrastructure planning professionally
 Company Scenario

Vantix Technologies is a newly established software development company with 20 employees across four departments:

Department	Employees
Information Technology	5
Human Resources	4
Finance	5
Sales	6
TOTAL	20

The company currently has no computers, server, network, internet infrastructure, or security policies — the entire environment was designed from scratch for this project.

 Hardware Inventory Summary
Category	Highlights
End-user devices	14 desktops + 6 laptops (one device per employee)
Server	1 server running Ubuntu Server (file sharing, Git, internal apps)
Network core	1 router, 1 managed switch, 1 firewall
Wireless	2 Wireless Access Points for full floor coverage
Peripherals	2 network printers, 19 monitors (incl. dual-monitor setups for IT)
Power & storage	3 UPS units, 1 NAS storage device, 2 external backup drives

Full inventory with Asset IDs, quantities, and justification is in EnterpriseInfrastructurePlan.pdf (Part 2).

 Software Inventory Summary
Category	Software
Operating Systems	Windows 11 Pro (endpoints), Ubuntu Server 22.04 LTS (server)
Productivity	Microsoft Office 365 Business Standard
Development	VS Code, Git, GitHub Desktop, VirtualBox
Security	Microsoft Defender
Utilities	Google Chrome, AnyDesk, 7-Zip

Full inventory with versions, license types, and justification is in EnterpriseInfrastructurePlan.pdf (Part 3).

 Embedded Network Diagram
## Git Installation
![Git Installation](network_diagram.png)

The topology flows: Internet → ISP Modem → Router → Firewall → Core Switch, which then distributes wired connectivity to the Server, Network Printer, and NAS Storage, and both wired and wireless connectivity to the IT, HR, Finance, and Sales departments through the Wireless Access Point.

Source/exported files: diagrams/network_diagram.png · diagrams/network_diagram.pdf

 Technologies Used
Draw.io / diagramming tools – network topology design
Markdown – technical documentation (this README)
Microsoft Word / PDF – formal infrastructure plan deliverable
GitHub – version control and portfolio hosting
LinkedIn – professional portfolio sharing
 Challenges Encountered

The most challenging part of this project was balancing completeness with clarity in the network diagram — fitting the firewall, switch, access point, server, printer, and all four departments into one diagram that is still easy for a non-technical executive to read. Writing realistic, business-justified quantities for the hardware inventory (rather than arbitrary numbers) also required thinking through each department's actual daily workflow.

 Reflection

A full 300–500 word reflection covering what I learned, the most challenging task, why planning matters before deployment, and how this project will help me become a better System Administrator is included in Part 8 of EnterpriseInfrastructurePlan.pdf.

 References
Cisco Networking Academy — https://www.netacad.com
CompTIA Certifications — https://www.comptia.org/certifications
Red Hat Certified System Administrator (RHCSA) — https://www.redhat.com/en/services/certification/rhcsa
AWS Certified Solutions Architect — https://aws.amazon.com/certification/