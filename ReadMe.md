**Designing and Implementing a Network**

**Introduction**

This project aims to design and implement a comprehensive network solution that meets the requirements of a mid-sized enterprise. 

Leveraging the principles and skills acquired through the Cisco Certified Network Associate (CCNA) certification, this project will cover the planning, design, configuration, and deployment of a scalable and secure network.
The primary objectives of this project include:

1.	**Network Design:** Developing a detailed network topology that ensures optimal performance, scalability, and redundancy.
2.	**Implementation:** Configuring network devices such as routers, switches, and firewalls to establish a secure and efficient network.
3.	**Testing and Validation:** Conducting thorough testing to ensure the network meets the desired performance and security standards.
4.	**Documentation:** Providing comprehensive documentation of the network design, configurations, and testing procedures.
5.	**Presentation:** Preparing and delivering a professional presentation that outlines the project’s objectives, design process, implementation steps, and outcomes.

At the end of this project, I aim to deliver a network infrastructure that not only supports the current needs of the organization but is also adaptable to future growth and technological advancements.

**Part 1: Designing a Network.**

**Instructions**

1.	Design a logical network topology using Packet Tracer simulation software for a company as described in the scenario below. 
2.	Create an addressing table for their respective network design, listing IP configuration for all the devices based on the requirements given below.

**Scenario**

You have been approached by a medium-sized company to help them design and create their network infrastructure. The company consists of five departments: Administration, Marketing, Sales, HR, and IT Support. Your task is to create a proof of concept for the network you plan to build using the latest version of Packet Tracer. You need to design a logical topology diagram with Packet Tracer.

Administration	Marketing	Sales 	HR	IT Support
LAN 1	 LAN 2	 LAN 1	 LAN 2	 LAN 1	 LAN 1	LAN 1	LAN 2	LAN 3
1225	250	100	5	31	18	133	50	72

*Design Requirements*
1.	Configure all subnetting requirements.

a.	To minimize the wasted address space, use VLSM (Variable Length Subnet Mask).

b.	All the devices must have an IP address.

c.	Expect 25% growth of current IP requirements when determining the size of subnets. 

d.	Use 192.31.0.0 for internal addressing. 

e.	Use /30 subnets for all the WAN interfaces.

f.	Assign names to all the devices as per your naming convention. 

g.	Connect a file server to the edge router to simulate internet.

h.	Define VLANs, names and their network addresses.

i.	Configure at least one host to each LAN.

j.	Each department should have a dedicated router and switch. 

k.	Select a department that will use LACP EtherChannel for Layer 2 redundancy. 

l.	Select another department that will use PAgP EtherChannel for Layer 2 redundancy. 

m.	IT Support will have Layer 3 redundancy through HSRP Protocol. So, there will be two routers for the IT Support department. One will be the primary active router and the other will be the secondary standby router. 

n.	Choose any two departments where clients will receive IP configuration through a DHCP Server. Label them on the Packet Tracer topology.

o.	Create an addressing table based on your network topology. The addressing table will assist with design and development activities and is critical when configuring switches and routers. It should include all the devices such as routers, switches, PCs. 

**Addressing Table**

Device Name	

Interface	

IP Address	

Subnet Mask	

Gateway
				
The tables and supporting text will be part of the documentation delivered to the company. Before you commence with the implementation, the logical diagram and tables need to be approved by the company.

**Part 2: Network Implementation**

**Instructions**


**Requirements**
1.	**Perform switch configurations:**

**a.	Name all the switches.**

1.	Configure a login password and set it as cisco. 

2.	Configure an encrypted privileged password and set it as class.

3.	All passwords should be encrypted.

b.	**Create the VLANs as per your project design for all departments/divisions on all switches.**
Each LAN will use a separate VLAN ID.

c.	Configure access ports.

d.	Create trunk ports and assign the management VLAN as the native VLAN.

e.	Assign a static IP address to all the Switches.

2.	**Choose any two departments and configure switch security on their switches:**

a.	Configure port security on the access ports.

b.	Disable unused ports and move them to a separate VLAN.

c.	Configure access ports to add the learned MAC address to the running configuration.

d.	Allow ports to accept a maximum of two MAC addresses.

e.	Configure violation mode restrict.

f.	Configure DHCP snooping globally and for the configured VLANs.

g.	Limit access ports to a limited rate of  3 DHCP Packets per second.

h.	Configure trunking ports as trusted ports.

i.	Configure access ports for portfast and BPDU Guard.

3.	Configure LACP EtherChannel between switches as labeled in your project design.
4.	Configure PAgP EtherChannel between switches as labeled in your project design.
5.	Configure inter-VLAN routing as per your project design.
6.	Configure DHCP pools as mentioned in your project design with excluded address ranges for the servers and gateways. 
7.	Configure the IP configuration on all the devices as per the addressing table found in your project design. Router and switch interfaces must have an appropriate description configured.
8.	Configure a default static route pointing towards the web server on the edge router.
9.	Configure any two departments with static routing.
10.	Configure the remaining three departments with OSPF routing. 
11.	Configure HSRP to provide redundant gateways according to the project design. The active router should be configured with the highest priority and preemption.


