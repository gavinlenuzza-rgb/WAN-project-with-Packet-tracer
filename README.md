# WAN-project-with-Packet-tracer
<h2> The Business Problem</h2>

Digital Learning is a registered training organisation (RTO) that provides computing-related training
courses in Melbourne. The RTO is expanding with three more branches/sites in various cities of
Australia, i.e. Sydney, Canberra and Adelaide.

Melbourne branch (Headquarter) Ethernet LAN infrastructure already up and running and consists
of:

 118 workstations (including staff and student’s workstations)
 
 2 database servers
 
 5 printers
 
 8 Cisco Catalyst 2960-X Series 24 port switches
 
 1 Cisco 4331 Integrated Services Router
 
 IPv4 class C network address of 192.168.1.0/24 are in use
 
Also, the entire Ethernet LAN connected with Cat6 cable (no wireless setup)
For other branches, the proposed Ethernet LAN design details are below:</h2>
<h3>Sydney</h3>
 140 workstations (including staff and student’s workstations)
 2 database servers
 6 printers
 9 Cisco Catalyst 2960-X Series 24 port switches
 1 Cisco 4331 Integrated Services Router
 IP address scheme (i.e. class or version not decided yet)
 No wireless setup required at this stage. However, UTP Cat5e or 6 likely to be used to
connect entire Ethernet LAN
<h3>Canberra</h3>
 80 workstations (including staff and student’s workstations)
 1 database server
 4 printers
 5 Cisco Catalyst 2960-X Series 24 port switches
 1 Cisco 4331 Integrated Services Router
 IP address scheme (i.e. class or version not decided yet)
 No wireless setup required at this stage. However, UTP Cat5e or 6 likely to be used to
connect entire Ethernet LAN
<h3>Adelaide</h3>
 110 workstations (including staff and student’s workstations)
 1 database server
 5 printers
 6 Cisco Catalyst 2960-X Series 24 port switches
 1 Cisco 4331 Integrated Services Router
 IP address scheme (i.e. class or version not decided yet)
 No wireless setup required at this stage. However, UTP Cat5e or 6 likely to be used to
connect entire Ethernet LAN

The managing director of the RTO has hired your services to connect Sydney, Canberra and
Adelaide branches with Melbourne branch and provided you the following project guideline.

Design Ethernet LAN and Wide Area Networks IP addressing scheme for Sydney,
Canberra and Adelaide branches.

Converge each branch LAN with other branches by enabling and configuring routing on
every router

Before moving to the actual design and implementation phase, the managing director provided you
a simulated design (as shown in Figure 1) of the proposed network which will assist you in
understanding the entire network topology. 

<h2>Network Diagram</h2>
<img width="601" height="351" alt="figure 1 scenario" src="https://github.com/user-attachments/assets/c826a3b9-3d5e-424f-8b0b-84d674c8c4e7" />



Details of the proposed topology are as follows:
- There are 4 routers, one for each branch. HQ-Melbourne is the edge router for the
Melbourne branch. B-Sydney is the edge router for the Sydney branch. B-Canberra is the
edge router for the Canberra branch. B-Adelaide is the edge router for the Adelaide
branch.
- Altogether, there are four Local Area Networks (LANs) and three Wide Area Networks
(WANs).
- Melbourne LAN is connected to the HQ-Melbourne router.
- Sydney LAN is connected to the B-Sydney router.
- Canberra LAN is connected to the B-Canberra router.
- Adelaide LAN is connected to the B-Adelaide router.

  <h2>Requirement</h2>
You need to configure and verify the proposed network in a simulated environment and ensure that
it is ready for actual implementation. 

<h2>IP Address Scheme</h2>
<img width="637" height="399" alt="Ip Address scheme" src="https://github.com/user-attachments/assets/2a01c41a-f800-40a8-bffe-f6dac0012caa" />

<img width="626" height="300" alt="Ip Address scheme part 2" src="https://github.com/user-attachments/assets/f3493df4-fa62-4e8a-8ee7-960defce8edc" />

<h2>Ethernet interface of end devices</h2>

A-PC1

<img width="551" height="591" alt="A-PC1" src="https://github.com/user-attachments/assets/84a9bdee-4939-44d8-a5f4-c1598af11318" />

C-PC1

<img width="602" height="538" alt="C-PC1" src="https://github.com/user-attachments/assets/733a22a6-4f42-4ffc-ba7a-6d12f7527671" />

M-PC1

<img width="549" height="582" alt="M-PC1" src="https://github.com/user-attachments/assets/2832ce8d-f72d-49a4-950c-a089a13f4f5c" />

S-PC1

<img width="555" height="591" alt="S-PC1" src="https://github.com/user-attachments/assets/2c0f13da-1fb7-46d8-8438-8fec787593c4" />

B-Adelaide

<img width="563" height="531" alt="B-Adelaide" src="https://github.com/user-attachments/assets/3df18357-3528-43ff-8ed5-a4fc29187957" />


B-Canbera

<img width="543" height="586" alt="B-Canbera" src="https://github.com/user-attachments/assets/495f67ac-ae2b-4a63-80a2-6a10607b6e50" />

B-Melbourne

<img width="550" height="575" alt="B-Melbourne" src="https://github.com/user-attachments/assets/442595df-2b31-4458-ae76-33284b249619" />

B-Sydney

<img width="557" height="593" alt="B-Sydney" src="https://github.com/user-attachments/assets/93d435ac-a7c2-406e-a8f3-f3f2f1907300" />


<h2>Basic Router Config</h2>
Details

<img width="605" height="96" alt="Basic router config" src="https://github.com/user-attachments/assets/1b2e27bd-6eaf-4a10-aa71-be9ad7f47594" />

Implementation

<img width="507" height="931" alt="B-Melb router config" src="https://github.com/user-attachments/assets/5c696f36-d0e5-4fa9-bdb6-e4251f72165a" />

Message of the day

<img width="468" height="645" alt="B-Melb router config motd" src="https://github.com/user-attachments/assets/0efa74c5-ecc8-4bd6-a1a6-2923b7448b06" />

<h2>Conbfigure OSPFv2</h2>

B-Adelaide

<img width="558" height="588" alt="Configure OSPFv2 Adelaide" src="https://github.com/user-attachments/assets/9af52db6-a702-4980-bb26-9195d81f605d" />

Verify OSPFv2 settings

<img width="561" height="589" alt="Verify OSPFv2 Adelaide" src="https://github.com/user-attachments/assets/f41c1e4b-3230-42e2-8a3c-6053e34e5062" />



