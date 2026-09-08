# Google Networking Roadmap

Status: In progress

What is  a network? a group of connected device , overall infrastructure 

![image.png](Google%20Networking%20Roadmap/image.png)

key terms 

- A  Hub : dumb and stupid , for security its really bad
- Switch
- Firewall : 1st line of defense
- Router
- Modem
- Server : a device provide or serve information for the client ( pc , phone etc)
- Client

![image.png](Google%20Networking%20Roadmap/image%201.png)

Key notes

# Network components, devices, and diagrams

**0:45/7:34**

In this reading, you will review network devices and connections and investigate a simple network diagram similar to those used every day by network security professionals.

A foundational understanding of network architecture, sometimes referred to as network design, will help you as you learn about security vulnerabilities inherent in all networks and how malicious actors attempt to exploit them. Let’s get started!

## **Network devices**

Network devices maintain information and services for users of a network. These devices connect over wired and wireless connections. After establishing a connection to the network, the devices send data packets. The data packets provide information about the source and the destination of the data.  This is how the information is sent and received via different devices on a network.

The network is the overall infrastructure that allows devices to communicate with each other. Network devices are specialized vehicles like routers and switches that manage what is being sent and received over the network. Additionally, devices like computers and phones connect to the network via network devices.

[](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/s-oBYPbLT42rx92K21cvxQ_611ef444b75147a5a6e61d82c34b0df1_9i07czTUt71fHdJt2WJV-5cS3YvI7Y1YQdOBF4c19c2wYkhrIu_6f5gYEgtzAKr8DArrVLx6QY6AQNHpMTmD410f6kyDVYNdP1x36o6lrmsv_CRG8iTBfcIZz4FA-g01ceMoYuXTJjCbvwf38YBSWVwB?expiry=1785951389846&hmac=-Mi_e7bPH3kOMOtfwMzNemqd47nHnMq0XZ2MFBt66vQ)

**Note:** In this diagram, a **router** connects to the internet through a **modem**, which is provided by your internet service provider (ISP). The firewall is a security device that monitors incoming and outgoing traffic on your network. The router then directs traffic to the devices on your home network, which can include computers, laptops, smartphones, tablets, printers, and other devices. You can imagine here that the server is a file server. All devices on this network can access the files in this **server**. This diagram also includes a **switch** which is an optional device that can be used to connect more devices to your network by providing additional ports and Ethernet connections. Additionally, there are 2 routers connected to the switch here for load balancing purposes which will improve the performance of the network.

### **Devices and desktop computers**

Most internet users are familiar with everyday devices, such as personal computers, laptops, mobile phones, and tablets. Each device and desktop computer has a unique MAC address and IP address, which identify it on the network. They also have a network interface that sends and receives data packets. These devices can connect to the network via a hard wire or a wireless connection.

### **Firewalls**

A **firewall** is a network security device that monitors traffic to or from your network. It is like your first line of defense. Firewalls can also restrict specific incoming and outgoing network traffic. The organization configures the security rules of the firewall. Firewalls often reside between the secured and controlled internal network and the untrusted network resources outside the organization, such as the internet. Remember, though, firewalls are just one line of defense in the cybersecurity landscape.

### **Servers**

**Servers** provide information and services for devices like computers, smart home devices, and smartphones on the network. The devices that connect to a server are called clients. The following graphic outlines this model, which is called the client-server model. In this model, clients send requests to the server for information and services. The server performs the requests for the clients. Common examples include DNS servers that perform domain name lookups for internet sites, file servers that store and retrieve files from a database, and corporate mail servers that organize mail for a company.

[](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/yEzpFYBkSWChuqHQuw5-SA_47876296b9c140229777d37bc916bff1_DVEYhkRb2cM57vspz3iQIbbBaOfDTWTukQLteY2SDv_MAofv-SbuGazdECwDkbJneVXdDvAW6-CuMSMbYLZJVdkUm5b9k0YJd7m9NVDbEZzLgBhO7_0eq30pRJkkUl-QHu97fSitfr2Lva1bPsTd431k?expiry=1785951389846&hmac=-9mFwQlkzJN-ukWwldvH8IVrGnPKr-rHmBdALQLxB9E)

### **Hubs and switches**

Hubs and switches both direct traffic on a local network. A **hub** is a device that provides a common point of connection for all devices directly connected to it. Hubs additionally repeat all information out to all ports. From a security perspective, this makes hubs vulnerable to eavesdropping. For this reason, hubs are not used as often on modern networks; most organizations use switches instead. Hubs are more commonly used for a limited network setup like a home office.

Switches are the preferred choice for most networks. A **switch** forwards packets between devices directly connected to it. They analyze the destination address of each data packet and send it to the intended device. Switches maintain a MAC address table that matches MAC addresses of devices on the network to port numbers on the switch and forwards incoming data packets according to the destination MAC address. Switches are a part of the data link layer in the TCP/IP model. Overall, switches improve performance and security.

### **Routers**

**Routers** connect networks and direct traffic, based on the IP address of the destination network. Routers allow devices on different networks to communicate with each other. In the TCP/IP model, routers are a part of the network layer. The IP address of the destination network is contained in the IP header. The router reads the IP header information and forwards the packet to the next router on the path to the destination. This continues until the packet reaches the destination network. Routers can also include a firewall feature that allows or blocks incoming traffic based on information in the transmission. This stops malicious traffic from entering the private network and damaging the local area network.

### **Modems and wireless access points**

**Modems** usually connect your home or office with an internet service provider (ISP). ISPs provide internet connectivity via telephone lines, coaxial cables, or fiber optic cables. Modems receive transmissions or digital signals from the internet and convert them into a digital format compatible with the physical connection provided by your ISP. Usually, modems connect to a router that takes the decoded transmissions and sends them on to the local network.

**Note:** Enterprise networks used by large organizations to connect their users and devices often use other broadband technologies to handle high-volume traffic, instead of using a modem.

[](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/6gFK3i1wRCyopAF5k1j0HQ_c8d352d18c8e4474941916da8fed74f1_GGmNcX8TiMojwILA_9er2cddFq573EvzkLIBJWj8Bpx5asAiGYLNe-aPI6ZluB_5ub9YgBHeHF5xMvQ52k5VknA8RtTVa033ZN5juPaHECodnA1W0ZhlbBJmWbgXrpomHeRypDrDT36bR8LFLRUN4Kxd?expiry=1785951389846&hmac=4tCMU4FO8hLspfGm5rF9uudyf2ZxTuFHPZ2m_29BMQU)

**Wireless access point**

A **wireless access point** sends and receives digital signals over radio waves creating a wireless network. Devices with wireless adapters connect to the access point using Wi-Fi. **Wi-Fi** refers to a set of standards that are used by network devices to communicate wirelessly. Wireless access points and the devices connected to them use Wi-Fi protocols to send data through radio waves where they are sent to routers and switches and directed along the path to their final destination.

[](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/8vl7L2RlSvGkk3LvXaMeKg_6a15bfb726f541d38671388c13b052f1_XU9XxDWBAwQu9gCYs4ZbRB4Do3xxXScibznS8UvafzSyYJoW9JpmUjL8VNbhYvmNmvmgP9x6AwGltYH7SnkcuyJjEGQNsFLvyeyun2-GdCqjHnXbExJgx67JoFd9KMohmA2xv462hh3O2xkvqhl1kX-z?expiry=1785951389846&hmac=OeFUlmdCEk7Uq9TC61oDVeMGl728FnLjJBROOvI_PMw)

## **Using network diagrams as a security analyst**

Network diagrams allow network administrators and security personnel to imagine the architecture and design of their organization’s private network.

**Network diagrams** are maps that show the devices on the network and how they connect. Network diagrams use small representative graphics to portray each network device and dotted lines to show how each device connects to the other. By studying network diagrams, security analysts develop and refine their strategies for securing network architectures.

[](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/v540rACBSUepbsQcE4s3PQ_3b799a13034d42938c980d7c473725f1_2SOA6jNuKUowAynp64ms-agTTUcxt1xas4SFTTAcKU-JfqJHyG2vzmM7qgqMh4J_Euwmri_t3G_CUXydGZRlmV4EZABYDusKE7pBnNWi5gZ_fUbiAetmRiQWL3cMO2iRWDtjtAPMazNxnmT-i5pWmPAe?expiry=1785951389846&hmac=Pcc0rQrwArnPy1uVXJ6Et2e5l2TSWZvcFZE0eBbN_qk)

## **Key takeaways**

In the client-server model, the client requests information and services from the server, and the server performs the requests for the clients. Network devices include routers, workstations, servers, hubs, switches, and modems. Security analysts use network diagrams to visualize network architecture.

- MAC address
- IP address

Explained like 5 

- 

### 1. MAC Address: Your Physical Home Address

Think of a **MAC address** like the **GPS coordinates or physical location of your home** (or the unique fingerprint stamped on your computer's network card when it was built in the factory).

- **Permanent:** It never changes. No matter where you move your computer—to a coffee shop, your house, or another country—its MAC address stays the exact same.
- **Unique:** No two devices in the entire world have the exact same MAC address.

### 2. IP Address: Your Mailing Address / Phone Number

Think of an **IP address** like the **mailing address or phone number** given to you by the place where you are connected right now.

- **Temporary / Dynamic:** It can change! When you plug your laptop into your home Wi-Fi, it gets one IP address. When you take your laptop to a coffee shop, the coffee shop gives it a completely different IP address.
- **Routing:** It tells the internet *where* to send your messages so they actually reach your specific neighborhood and network.

### How They Work Together (The Analogy)

Imagine someone wants to send you a package:

- The postal service uses your **IP Address** to figure out which **city, street, and house** to bring the package to.
- Once the mail carrier arrives at the front door, they use the **MAC Address** (your face/fingerprint) to make sure they hand the box to **you specifically**, and not your roommate or neighbor!

Explained like 5 

A Hub : dumb and stupid , for security its really bad  , why they invented this the?

# 

You hit the nail right on the head! In terms of security and traffic management, hubs are pretty much the "dumb and stupid" grandparents of network hardware.

If a hub gets a piece of data intended for Computer A, it doesn't know who Computer A is—so it literally screams that data out to **every single port on the device** (Computer B, Computer C, the printer, the smart toaster). Everyone receives it, inspects it, and decides whether to drop it or keep it. For security, that means anyone on a hub can easily eavesdrop on *all* network traffic.

So, why on Earth did engineers invent them?

### 1. Simple Silicon Was Cheap (and Early Tech Was Primitive)

Back in the 1980s and early 1990s, microchips were expensive, weak, and slow.

- A **Hub** is just a simple physical layer device (Layer 1). It doesn't need a CPU, memory, or logic to read packet headers. It takes electrical signals from one wire and duplicates them to all the other wires. It’s basically a glorified, powered extension cord.
- A **Switch** (Layer 2), on the other hand, needs a computer processor, dynamic RAM, and specialized chips (ASICs) to inspect packet headers, read MAC addresses, and build an internal memory lookup table (MAC address table). 40 years ago, building a switch was wildly complex and insanely expensive.

### 2. Switches Used to Cost a Fortune

When networking was first taking off in offices:

- A **Hub** might have cost **$50 to $100**.
- A **Switch** with similar ports could cost **thousands of dollars**.

For a small business that just wanted 5 computers to share an internet connection or print documents, paying thousands of dollars for a switch didn't make financial sense. Hubs were the budget-friendly solution that made mass networking affordable.

### 3. Cyber Security Wasn't a Priority Yet

When hubs were created, the internet was mostly used by universities, government researchers, and a small number of corporations.

- **Trust by default:** Early networks were built on the assumption that if someone had physical access to plug a cable into a wall, they were an authorized, trusted user.
- Nobody was thinking about packet sniffing, MITM (Man-in-the-Middle) attacks, or internal corporate espionage when the physical protocols were being drawn up.

### 4. Networks Were Slow (No Traffic Jams Yet)

In the era of 10 Mbps Ethernet, networks weren't streaming 4K video or moving gigabytes of cloud data. The amount of network noise and "collisions" (when two devices talk at the exact same time on a hub and mess up the signal) was manageable for tiny office setups.

### Summary

Hubs weren't invented because engineers were bad at their jobs—they were invented because **they were the cheapest, simplest way to connect computers given the limited tech of the time.**

As chip manufacturing got cheaper in the late 1990s and early 2000s, switches became affordable, network security became vital, and hubs were quickly tossed into the garbage bin of tech history!

**Eavesdropping** is when a third kid secretly hides behind a bookshelf or presses their ear against the wall to **listen in on the conversation without being invited**.

Cloud Computing

![image.png](Google%20Networking%20Roadmap/image%202.png)

Review notes about CSP (Cloud Service Providers)

**Test your knowledge: Introduction to networks**

![image.png](Google%20Networking%20Roadmap/image%203.png)

![image.png](Google%20Networking%20Roadmap/image%204.png)

### ***Introduction to network communication***

![image.png](Google%20Networking%20Roadmap/image%205.png)

![image.png](Google%20Networking%20Roadmap/image%206.png)

4 layers of TCP/IP model

NITA

 Network layer >  Internet layer >  Transport layer>Access  

![image.png](Google%20Networking%20Roadmap/image%207.png)

In this reading, you will build on what you have learned about the Transmission Control Protocol/Internet Protocol (TCP/IP) model, consider the differences between the Open Systems Interconnection (OSI) model and TCP/IP model, and learn how they’re related. Then, you’ll review each layer of the TCP/IP model and go over common protocols used in each layer.

As a security professional, it's important that you understand the TCP/IP model because it describes the functions of various network protocols. The TCP/IP model is based on the TCP/IP protocols suite that includes all network protocols that support the main TCP/IP protocol. To reiterate from previous lessons, a network protocol, also known as an internet protocol, is a set of standards used for routing and addressing data packets as they travel between devices on a network. In this reading, you will learn which network protocols operate on which communication layers of the TCP/IP model. The two most common models available are the TCP/IP and the OSI model. These models are a representative guideline of how hosts communicate across a network. The examples provided in this course will follow the TCP/IP model.

## **The TCP/IP model**

The **TCP/IP model** is a framework used to visualize how data is organized and transmitted across a network. This model helps network engineers and network security analysts conceptualize processes on the network and communicate where disruptions or security threats occur.

The TCP/IP model has four layers: the **network access** layer, internet layer, transport layer, and application layer. When troubleshooting issues on the network, security professionals can analyze which layers were impacted by an attack based on what processes were involved in an incident.

![The four layers of the TCP/IP model labeled application layer, transport layer, internet layer, and network access layer](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/H9jj1YSsSDKlU8c8qzOgsQ_89f77799b50040b08911a8de1012e2f1_CS_R-210_S33G011-edited.png?expiry=1786069765767&hmac=60VKp0jTzgybE46PsqWI9v6mfKrWNLi-c9j9AuNrxbs)

## **Network access layer**

The network access layer, sometimes called the data link layer, deals with the creation of data packets and their transmission across a network. This layer corresponds to the physical hardware involved in network transmission. Hubs, modems, cables, and wiring are all considered part of this layer. The address resolution protocol (ARP) is part of the network access layer. Since MAC addresses are used to identify hosts on the same physical network, ARP is needed to map IP addresses to MAC addresses for local network communication.

## **Internet layer**

The internet layer, sometimes referred to as the network layer, is responsible for ensuring the delivery to the destination host, which potentially resides on a different network. It ensures IP addresses are attached to data packets to indicate the location of the sender and receiver. The internet layer also determines which protocol is responsible for delivering the data packets and ensures the delivery to the destination host. Here are some of the common protocols that operate at the internet layer:

- **Internet Protocol (IP)**. IP sends the data packets to the correct destination and relies on the Transmission Control Protocol/User Datagram Protocol (TCP/UDP) to deliver them to the corresponding service. IP packets allow communication between two networks. They are routed from the sending network to the receiving network. TCP in particular retransmits any data that is lost or corrupt.
- **Internet Control Message Protocol (ICMP)**. The ICMP shares error information and status updates of data packets. This is useful for detecting and troubleshooting network errors. The ICMP reports information about packets that were dropped or that disappeared in transit, issues with network connectivity, and packets redirected to other routers.

## **Transport layer**

The transport layer is responsible for delivering data between two systems or networks and includes protocols to control the flow of traffic across a network. TCP and UDP are the two transport protocols that occur at this layer.

### **Transmission Control Protocol**

The **Transmission Control Protocol (TCP)** is an internet communication protocol that allows two devices to form a connection and stream data. It ensures that data is reliably transmitted to the destination service. TCP contains the port number of the intended destination service, which resides in the TCP header of a TCP/IP packet.

### **User Datagram Protocol**

The **User Datagram Protocol (UDP)** is a connectionless protocol that does not establish a connection between devices before transmissions. It is used by applications that are not concerned with the reliability of the transmission. Data sent over UDP is not tracked as extensively as data sent using TCP. Because UDP does not establish network connections, it is used mostly for performance sensitive applications that operate in real time, such as video streaming.

## **Application layer**

The application layer in the TCP/IP model is similar to the application, presentation, and session layers of the OSI model. The application layer is responsible for making network requests or responding to requests. This layer defines which internet services and applications any user can access. Protocols in the application layer determine how the data packets will interact with receiving devices. Some common protocols used on this layer are:

- Hypertext transfer protocol (HTTP)
- Simple mail transfer protocol (SMTP)
- Secure shell (SSH)
- File transfer protocol (FTP)
- Domain name system (DNS)

Application layer protocols rely on underlying layers to transfer the data across the network.

## **TCP/IP model versus OSI model**

![The TCP/IP model next to the OSI model](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/RbNt47PDRTGJZ6q_QtaNMg_9b9098ac04e84c2d8ad04b220c5456f1_CS_R-210_TCP-vs-OSI.png?expiry=1786069765767&hmac=MgbSlkGV4gJM8ZECFlKDVDMNshfcrB3zVRi_KuMGv-c)

The **OSI** visually organizes network protocols into different layers. Network professionals often use this model to communicate with each other about potential sources of problems or security threats when they occur.

The TCP/IP model combines multiple layers of the OSI model. There are many similarities between the two models. Both models define standards for networking and divide the network communication process into different layers. The TCP/IP model is a simplified version of the OSI model.

## **Key takeaways**

Both the TCP/IP and OSI models are conceptual models that help network professionals visualize network processes and protocols in regards to data transmission between two or more systems. The TCP/IP model contains four layers, and the OSI model contains seven layers.

DO THE ASSIGNMENT

**IP addresses and network communication**

![image.png](Google%20Networking%20Roadmap/image%208.png)

IPV4 AND IPV6

# Components of network layer communication

**0:21/7:35**

In the reading about the [OSI model](https://www.coursera.org/learn/networks-and-network-security/supplement/YbKL0/the-osi-model-explained), you learned about the seven layers of the OSI model that are used to conceptualize the way data is transmitted across the internet. In this reading, you will learn more about operations that take place at layer 3 of the OSI model: the network layer.

## **Operations at the network layer**

Functions at the network layer organize the addressing and delivery of data packets across the network from the host device to the destination device. This includes directing the packets from one router to another router across the internet, till it reaches the internet protocol (IP) address of the destination network. The destination IP address is contained within the header of each data packet. This address will be stored for future routing purposes in  routing tables along the packet’s path to its destination.

All data packets include an IP address. A data packet is also referred to as an IP packet for TCP connections or a datagram for UDP connections. A router uses the IP address to route packets from network to network based on information contained in the IP header of a data packet. Header information communicates more than just the address of the destination. It also includes information such as the source IP address, the size of the packet, and which protocol will be used for the data portion of the packet.

## **Format of an IPv4 packet**

![An IP packet divided into two parts: a section on the left marked “header,” and section on the right marked “data”](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/NHNCeVwQQCCcfSTfEUTolg_afd9af6faf854e3db824471a7f2e56f1_CS_R-044_Edited_IP-packet-header-and-data-final.png?expiry=1786070887713&hmac=z7hBXmQi3SqGS9hCqiVwPWmZ1pBk8tOq8xPcsmSASS8)

Next, you can review the format of an IP version 4 (IPv4) packet and review a detailed graphic of the packet header. An IPv4 packet is made up of two sections, the header and the data:

- An IPv4 header format is determined by the IPv4 protocol and includes the IP routing information that devices use to direct the packet. The size of the IPv4 header ranges from 20 to 60 bytes. The first 20 bytes are a fixed set of information containing data such as the source and destination IP address, header length, and total length of the packet. The last set of bytes can range from 0 to 40 and consists of the options field.
- The length of the data section of an IPv4 packet can vary greatly in size. However, the maximum possible size of an IPv4 packet is 65,535 bytes. It contains the message being transferred over the internet, like website information or email text.

![Diagram of an IPv4 packet header, 13 fields, and bit size](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ZlTJLULmT_-iQusFt5gHLA_34841ae20ac344f4a0248aebe8f0d6f1_CS_R-044_Edited_Pv4-packet-header-14-field.png?expiry=1786070887713&hmac=V8RuWmrXxe9GGVrE-2mf4Qm2UwF6xgi0uV3Dwtqcq-I)

There are 13 fields within the header of an IPv4 packet:

- **Version (VER):** This 4 bit component tells receiving devices what protocol the packet is using. The packet used in the illustration above is an IPv4 packet.
- **IP Header Length (HLEN or IHL):** HLEN is the packet’s header length. This value indicates where the packet header ends and the data segment begins.
- **Type of Service (ToS):** Routers prioritize packets for delivery to maintain quality of service on the network. The ToS field provides the router with this information.
- **Total Length:** This field communicates the total length of the entire IP packet, including the header and data. The maximum size of an IPv4 packet is 65,535 bytes.
- **Identification:** IPv4 packets can be up to 65, 535 bytes, but most networks have a smaller limit. In these cases, the packets are divided, or fragmented, into smaller IP packets. The identification field provides a unique identifier for all the fragments of the original IP packet so that they can be reassembled once they reach their destination.
- **Flags:** This field provides the routing device with more information about whether the original packet has been fragmented and if there are more fragments in transit.
- **Fragmentation Offset:** The fragment offset field tells routing devices where in the original packet the fragment belongs.
- **Time to Live (TTL):** TTL prevents data packets from being forwarded by routers indefinitely. It contains a counter that is set by the source. The counter is decremented by one as it passes through each router along its path. When the TTL counter reaches zero, the router currently holding the packet will discard the packet and return an ICMP Time Exceeded error message to the sender.
- **Protocol:** The protocol field tells the receiving device which protocol will be used for the data portion of the packet.
- **Header Checksum:** The header checksum field contains a checksum that can be used to detect corruption of the IP header in transit. Corrupted packets are discarded.
- **Source IP Address:** The source IP address is the IPv4 address of the sending device.
- **Destination IP Address:** The destination IP address is the IPv4 address of the destination device.
- **Options:** The options field allows for security options to be applied to the packet if the HLEN value is greater than five. The field communicates these options to the routing devices.

## **Difference between IPv4 and IPv6**

In an earlier part of this course, you learned about the history of IP addressing. As the internet grew, it became clear that all of the IPv4 addresses would eventually be depleted; this is called IPv4 address exhaustion. At the time, no one had anticipated how many computing devices would need an IP address. IPv6 was developed to mitigate IPv4 address exhaustion and other related concerns.

Some of the key differences between IPv4 and IPv6 include the length and the format of the addresses. IPv4 addresses are made up of four decimal numbers separated by periods, each number ranging from 0 to 255. Together the numbers span 4 bytes, and allow for up to 4.3 billion possible addresses. An example of an IPv4 address would be: 198.51.100.0. IPv6 addresses are made of eight hexadecimal numbers separated by colons, each number consisting of up to four hexadecimal digits. Together, all numbers span 16 bytes, and allow for up to 340 undecillion addresses (340 followed by 36 zeros). An example of an IPv6 address would be: 2002:0db8:0000:0000:0000:ff21:0023:1234.

***Note:** to represent one or more consecutive sets of all zeros, you can replace the zeros with a double colon "::", so the above IPv6 address would be "*2002:0db8::ff21:0023:1234."

There are also some differences in the layout of an IPv6 packet header. The IPv6 header format is much simpler than IPv4. For example, the IPv4 Header includes the IHL, Identification, and Flags fields, whereas the IPv6 does not. The IPv6 header only introduces the Flow Label field, where the Flow Label identifies a packet as requiring special handling by other IPv6 routers.

![Side by side diagrams of an IPv4 packet header and a simplified IPv6 packet](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/PNld6YkmQNWyhZjFFHvC-Q_eb474e5ee3b3416fbc06a639503342f1_CS_R-044_IPv4-and-IPv6.png?expiry=1786070887713&hmac=D_CFeqgwq8tu4AQS-k5fww_qcwLwv5NEyi0cToDCX44)

There are some important security differences between IPv4 and IPv6. IPv6 offers more efficient routing and eliminates private address collisions that can occur on IPv4 when two devices on the same network are attempting to use the same address.

## **Key takeaways**

Analyzing the different fields in an IP data packet can be used to find out important security information about the packet. Some examples of security-related information found in IP address packets are: where the packet is coming from, where it’s going, and which protocol it’s using. Understanding the data in an IP data packet will allow you to make critical decisions about the security implications of packets that you inspect.

# Glossary terms from module 1

**0:13/2:25**

## **Terms and definitions from Course 3, Module 1**

**Bandwidth:** The maximum data transmission capacity over a network, measured by bits per second

**Cloud computing:** The practice of using remote servers, application, and network services that are hosted on the internet instead of on local physical devices

**Cloud network:** A collection of servers or computers that stores resources and data in remote data centers that can be accessed via the internet

**Data packet:** A basic unit of information that travels from one device to another within a network

**Hub:** A network device that broadcasts information to every device on the network

**Internet Protocol (IP):** A set of standards used for routing and addressing data packets as they travel between devices on a network

**Internet Protocol (IP) address:** A unique string of characters that identifies the location of a device on the internet

**Local Area Network (LAN):** A network that spans small areas like an office building, a school, or a home

**Media Access Control (MAC) address:** A unique alphanumeric identifier that is assigned to each physical device on a network

**Modem:** A device that connects your router to the internet and brings internet access to the LAN

**Network:** A group of connected devices

**Open systems interconnection (OSI) model:** A standardized concept that describes the seven layers computers use to communicate and send data over the network

**Packet sniffing:** The practice of capturing and inspecting data packets across a network

**Port:** A software-based location that organizes the sending and receiving of data between devices on a network.

**Router:** A network device that connects multiple networks together.

**Speed:** The rate at which a device sends and receives data, measured by bits per second

**Switch:** A device that makes connections between specific devices on a network by sending and receiving data between them.

**TCP/IP model:** A framework used to visualize how data is organized and transmitted across a network.

**Transmission Control Protocol (TCP):** An internet communication protocol that allows two devices to form a connection and stream data

**User Datagram Protocol (UDP):** A connectionless protocol that does not establish a connection between devices before transmissions

**Wide Area Network (WAN):** A network that spans a large geographic area like a city, state, or country

**Network Protocols . Hand shake**

![image.png](Google%20Networking%20Roadmap/image%209.png)

In this section of the course, you learned about network protocols and how they organize communication over a network. This reading will discuss network protocols in more depth and review some basic protocols that you have learned previously. You will also learn new protocols and discuss some of the ways protocols are involved in network security.

## **Overview of network protocols**

A **network protocol** is a set of rules used by two or more devices on a network to describe the order of delivery and the structure of data. Network protocols serve as instructions that come with the information in the data packet. These instructions tell the receiving device what to do with the data. Protocols are like a common language that allows devices all across the world to communicate with and understand each other.

Even though network protocols perform an essential function in network communication, security analysts should still understand their associated security implications. Some protocols have vulnerabilities that malicious actors exploit. For example, a nefarious actor could use the Domain Name System (DNS) protocol, which resolves web addresses to IP addresses, to divert traffic from a legitimate website to a malicious website containing malware. You’ll learn more about this topic in upcoming course materials.

## **Three categories of network protocols**

Network protocols can be divided into three main categories: communication protocols, management protocols, and security protocols. There are dozens of different network protocols, but you don’t need to memorize all of them for an entry-level security analyst role. However, it’s important for you to know the ones listed in this reading.

### **Communication protocols**

Communication protocols govern the exchange of information in network transmission. They dictate how the data is transmitted between devices and the timing of the communication. They also include methods to recover data lost in transit. Here are a few of them.

- **Transmission Control Protocol (TCP)** is an internet communication protocol that allows two devices to form a connection and stream data. TCP uses a three-way handshake process. First, the device sends a synchronize (SYN) request to a server. Then the server responds with a SYN/ACK packet to acknowledge receipt of the device's request. Once the server receives the final ACK packet from the device, a TCP connection is established. In the TCP/IP model, TCP occurs at the transport layer.
- **User Datagram Protocol (UDP)** is a connectionless protocol that does not establish a connection between devices before a transmission. This makes it less reliable than TCP. But it also means that it works well for transmissions that need to get to their destination quickly. For example, one use of UDP is for sending DNS requests to local DNS servers. In the TCP/IP model, UDP occurs at the transport layer.
- **Hypertext Transfer Protocol (HTTP)** is an application layer protocol that provides a method of communication between clients and website servers. HTTP uses port 80. HTTP is considered insecure, so it is being replaced on most websites by a secure version, called HTTPS that uses encryption from SSL/TLS for communication. However, there are still many websites that use the insecure HTTP protocol. In the TCP/IP model, HTTP occurs at the application layer.
- **Domain Name System (DNS)** is a protocol that translates internet domain names into IP addresses. When a client computer wishes to access a website domain using their internet browser, a query is sent to a dedicated DNS server. The DNS server then looks up the IP address that corresponds to the website domain. DNS normally uses UDP on port 53. However, if the DNS reply to a request is large, it will switch to using the TCP protocol. In the TCP/IP model, DNS occurs at the application layer.

### **Management Protocols**

The next category of network protocols is management protocols. Management protocols are used for monitoring and managing activity on a network. They include protocols for error reporting and optimizing performance on the network.

- **Simple Network Management Protocol (SNMP)** is a network protocol used for monitoring and managing devices on a network. SNMP can reset a password on a network device or change its baseline configuration. It can also send requests to network devices for a report on how much of the network’s bandwidth is being used up. In the TCP/IP model, SNMP occurs at the application layer.
- **Internet Control Message Protocol (ICMP)** is an internet protocol used by devices to tell each other about data transmission errors across the network. ICMP is used by a receiving device to send a report to the sending device about the data transmission. ICMP is commonly used as a quick way to troubleshoot network connectivity and latency by issuing the “ping” command on a Linux operating system. In the TCP/IP model, ICMP occurs at the internet layer.

### **Security Protocols**

Security protocols are network protocols that ensure that data is sent and received securely across a network. Security protocols use encryption algorithms to protect data in transit. Below are some common security protocols.

- **Hypertext Transfer Protocol Secure (HTTPS)** is a network protocol that provides a secure method of communication between clients and website servers. HTTPS is a secure version of HTTP that uses secure sockets layer/transport layer security (SSL/TLS) encryption on all transmissions so that malicious actors cannot read the information contained. HTTPS uses port 443. In the TCP/IP model, HTTPS occurs at the application layer.
- **Secure File Transfer Protocol (SFTP)** is a secure protocol used to transfer files from one device to another over a network. SFTP uses secure shell (SSH), typically through TCP port 22. SSH uses Advanced Encryption Standard (AES) and other types of encryption to ensure that unintended recipients cannot intercept the transmissions. In the TCP/IP model, SFTP occurs at the application layer. SFTP is used often with cloud storage. Every time a user uploads or downloads a file from cloud storage, the file is transferred using the SFTP protocol.

**Note:** The encryption protocols mentioned do not conceal the source or destination IP address of network traffic. This means a malicious actor can still learn some basic information about the network traffic if they intercept it.

## **Key takeaways**

The protocols you learned about in this reading are basic networking protocols that entry-level cybersecurity analysts should know. Understanding how protocols function on a network is essential. Cybersecurity analysts can leverage their knowledge of protocols to successfully mitigate vulnerabilities on a network and potentially prevent future attacks.

***System identification -08-08-2026***

**Firewalls and network security measures**

![image.png](Google%20Networking%20Roadmap/image%2010.png)

***Virtual private networks (VPNs)***

Encapsulation is a process performed by a VPN service that protects your data by wrapping sensitive data in other data packets.

![image.png](Google%20Networking%20Roadmap/image%2011.png)

![image.png](Google%20Networking%20Roadmap/image%2012.png)

***Security zones***

Security zones are a segment of a network that protects the internal network from the internet.

They are a part of a security technique called network segmentation that divides the network into segments.

![image.png](Google%20Networking%20Roadmap/image%2013.png)

Two types of security zones. 

First, there's the uncontrolled zone, which is any network outside of the organization's control, like the internet.

Then, there's the controlled zone, which is a subnet that protects the internal network from the uncontrolled zone.

![image.png](Google%20Networking%20Roadmap/image%2014.png)

![image.png](Google%20Networking%20Roadmap/image%2015.png)

![image.png](Google%20Networking%20Roadmap/image%2016.png)

# Subnetting and CIDR

**0:30/4:10**

Earlier in this course, you learned about network segmentation, a security technique that divides networks into sections. A private network can be segmented to protect portions of the network from the internet, which is an unsecured global network.

For example, you learned about the uncontrolled zone, the controlled zone, the demilitarized zone, and the restricted zone. Feel free to review the video about [security zones](https://www.coursera.org/learn/networks-and-network-security/lecture/GccYm/security-zones) for a refresher on how network segmentation can be used to add a layer of security to your organization’s network operations. Creating security zones is one example of a networking strategy called subnetting.

## **Overview of subnetting**

**Subnetting** is the process of taking one large network and **dividing it into several smaller, organized groups** called **subnets**. Think of it like this: If your company's network is a large city, each subnet is a distinct neighborhood within that city.

Subnetting divides up a network address range into smaller subnets within the network. These organized subnets are defined by the unique combination of the **IP address** and the **network mask** assigned to every device, effectively creating a "network within a network." Subnetting creates a network of devices to function as their own network. This makes the network more efficient and can also be used to create security zones. If devices on the same subnet communicate with each other, the switch changes the transmissions to stay on the same subnet, improving speed and efficiency of the communications.

[Two subnets for two networks connected to one router.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vzbgwk8-RoCJ8Ppet89raA_1a225a330b8b4eaeb4a2b8bc5baaaef1_qvNCswL7ECbUiKTyL6rjp35BTSD-bbfoAoajmAyy4hHvmBJwwr22RU8T5aGDunmwKb1kvZ5TneMbG-nngVlkPXF6W-BTMap_a6XP-kAy5jgW13XvT5OTSCmI7U9YVNX4JzC1qn-zCkiZSXhbKjm2zq7SESzmANYH17_p4jub1mNikwElbJZECK0VuM_4Yrwljgfgdx2VpNad7gx2lFHMiu01wfeRKp-sjRa_kQ?expiry=1786253943586&hmac=KjsUFNLqZm1i06hVVtypLqlB0gvqn4wgY153UM71lSc)

## **Classless Inter-Domain Routing notation for subnetting**

Classless Inter-Domain Routing (CIDR) is a method of assigning subnet masks to IP addresses to create a subnet. Classless addressing replaces classful addressing. Classful addressing was used in the 1980s as a system of grouping IP addresses into classes (Class A to Class E). Each class included a limited number of IP addresses, which were depleted as the number of devices connecting to the internet outgrew the classful range in the 1990s. Classless CIDR addressing expanded the number of available IPv4 addresses.

CIDR allows cybersecurity professionals to segment classful networks into smaller chunks. CIDR IP addresses are formatted like IPv4 addresses, but they include a slash (“/”) followed by a number at the end of the address, This extra number is called the IP network prefix.  For example, a regular IPv4 address uses the 198.51.100.0 format, whereas a CIDR IP address would include the IP network prefix at the end of the address, 198.51.100.0/24. This CIDR address encompasses all IP addresses between 198.51.100.0 and 198.51.100.255. The system of CIDR addressing reduces the number of entries in routing tables and provides more available IP addresses within networks. You can try converting CIDR to IPv4 addresses and vice versa through an online conversion tool, like [IPAddressGuide](https://www.ipaddressguide.com/cidr), for practice and to better understand this concept.

**Note:** For now, focus on understanding the concept of CIDR as a flexible addressing method used for modern subnetting. A deeper dive into the technical mathematics of CIDR is a valuable skill you can develop further in future training if needed.

## **Security benefits of subnetting**

Subnetting allows network professionals and analysts to create a network within their own network without requesting another network IP address from their internet service provider. This process uses network bandwidth more efficiently and improves network performance. Subnetting is one component of creating isolated subnetworks through physical isolation, routing configuration, and firewalls.

## **Key takeaways**

Subnetting is a common security strategy used by organizations. Subnetting allows organizations to create smaller networks within their private network. This improves the efficiency of the network and can be used to create security zones.

***Proxy servers***

The definition of a proxy server is a server that fulfills the request of a client by forwarding them on to other servers.

![image.png](Google%20Networking%20Roadmap/image%2017.png)

![image.png](Google%20Networking%20Roadmap/image%2018.png)

# Virtual networks and privacy

**0:06/6:33**

This section of the course covered a lot of information about network operations. You reviewed the fundamentals of network architecture and communication and can now use this knowledge as you learn how to secure networks. Securing a private network requires maintaining the confidentiality of your data and restricting access to authorized users.

In this reading, you will review several network security topics previously covered in the course, including virtual private networks (VPNs), proxy servers, firewalls, and security zones. You'll continue to learn more about these concepts and how they relate to each other as you continue through the course.

## **Common network protocols**

Network protocols are used to direct traffic to the correct device and service depending on the kind of communication being performed by the devices on the network. Protocols are the rules used by all network devices that provide a mutually agreed upon foundation for how to transfer data across a network.

There are three main categories of network protocols: communication protocols, management protocols, and security protocols.

1. Communication protocols are used to establish connections between servers. Examples include TCP, UDP, and Simple Mail Transfer Protocol (SMTP), which provides a framework for email communication.
2. Management protocols are used to troubleshoot network issues. One example is the Internet Control Message Protocol (ICMP).
3. Security protocols provide encryption for data in transit. Examples include IPSec and SSL/TLS.

Some other commonly used protocols are:

- HyperText Transfer Protocol (HTTP). HTTP is an application layer communication protocol. This allows the browser and the web server to communicate with one another.
- Domain Name System (DNS). DNS is an application layer protocol that translates, or maps, host names to IP addresses.
- Address Resolution Protocol (ARP). ARP is a network layer communication protocol that maps IP addresses to physical machines or a MAC address recognized on the local area network.

## **Wi-Fi**

This section of the course also introduced various wireless security protocols, including WEP, WPA, WPA2, and WPA3. WPA3 encrypts traffic with the Advanced Encryption Standard (AES) cipher as it travels from your device to the wireless access point. WPA2 and WPA3 offer two modes: personal and enterprise. Personal mode is best suited for home networks while enterprise mode is generally utilized for business networks and applications.

## **Network security tools and practices**

### **Firewalls (rule based access control)**

Previously, you learned that firewalls are network virtual appliances (NVAs) or hardware devices that inspect and can filter network traffic before it’s permitted to enter the private network. Traditional firewalls are configured with rules that tell it what types of data packets are allowed based on the port number and IP address of the data packet.

There are two main categories of firewalls.

- **Stateless:** A class of firewall that operates based on predefined rules and does not keep track of information from data packets.
- **Stateful:** A class of firewall that keeps track of information passing through it and proactively filters out threats. Unlike stateless firewalls, which require rules to be configured in two directions, a stateful firewall only requires a rule in one direction. This is because it uses a "state table" to track connections, so it can match return traffic to an existing session

Next generation firewalls (NGFWs) are the most technologically advanced firewall protection. They exceed the security offered by stateful firewalls because they include deep packet inspection (a kind of packet sniffing that examines data packets and takes actions if threats exist) and intrusion prevention features that detect security threats and notify firewall administrators. NGFWs can inspect traffic at the application layer of the TCP/IP model and are typically application aware. Unlike traditional firewalls that block traffic based on IP address and ports, NGFWs rules can be configured to block or allow traffic based on the application. Some NGFWs have additional features like Malware Sandboxing, Network Anti-Virus, and URL and DNS Filtering.

### **Proxy servers**

A proxy server is another way to add security to your private network. Proxy servers utilize network address translation (NAT) to serve as a barrier between clients on the network and external threats. Forward proxies handle queries from internal clients when they access resources external to the network. Reverse proxies function opposite of forward proxies; they handle requests from external systems to services on the internal network. Some proxy servers can also be configured with rules, like a firewall.  For example, you can create filters to block websites identified as containing malware.

### **Virtual Private Networks (VPN)**

A VPN is a service that encrypts data in transit and disguises your IP address. VPNs use a process called encapsulation. Encapsulation wraps your unencrypted data in an encrypted data packet, which allows your data to be sent across the public network while remaining anonymous. Enterprises and other organizations use VPNs to help protect communications from users’ devices to corporate resources. Some of these resources include servers or virtual machines that host business applications. Individuals also use VPNs to increase personal privacy. VPNs protect user privacy by concealing personal information, including IP addresses, from external servers. A reputable VPN also minimizes its own access to user internet activity by using strong encryption and other security measures. Organizations are increasingly using a combination of VPN and SD-WAN capabilities to secure their networks. A software-defined wide area network (SD-WAN) is a virtual WAN service that allows organizations to securely connect users to applications across multiple locations and over large geographical distances.

### **Key takeaways**

There are three main categories of network protocols: communication, management, and security protocols. In this reading, you learned the fundamentals of firewalls, proxy servers, and VPNs. More organizations are implementing a cloud-based approach to network security by incorporating a combination of VPN and SD-WAN capabilities as a service.

# VPN protocols: Wireguard and IPSec

**0:33/4:21**

A VPN, or virtual private network, is a network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you’re using a public network like the internet. VPNs provide a server that acts as a gateway between a computer and the internet. This server creates a path similar to a virtual tunnel that hides the computer’s IP address and encrypts the data in transit to the internet. The main purpose of a VPN is to create a secure connection between a computer and a network. Additionally, a VPN allows trusted connections to be established on non-trusted networks. VPN protocols determine how the secure network tunnel is formed. Different VPN providers provide different VPN protocols.

This reading will cover the differences between remote access and site-to-site VPNs, and two VPN protocols: WireGuard VPN and IPSec VPN. A VPN protocol is similar to a network protocol: It’s a set of rules or instructions that will determine how data moves between endpoints. An endpoint is any device connected on a network. Some examples of endpoints include computers, mobile devices, and servers.

## **Remote access and site-to-site VPNs**

Individual users use remote access VPNs to establish a connection between a personal device and a VPN server. Remote access VPNs encrypt data sent or received through a personal device. The connection between the user and the remote access VPN is established through the internet.

Enterprises use site-to-site VPNs largely to extend their network to other networks and locations. This is particularly useful for organizations that have many offices across the globe. IPSec is commonly used in site-to-site VPNs to create an encrypted tunnel between the primary network and the remote network. One disadvantage of site-to-site VPNs is how complex they can be to configure and manage compared to remote VPNs.

## **WireGuard VPN vs. IPSec VPN**

WireGuard and IPSec are two different VPN protocols used to encrypt traffic over a secure network tunnel. The majority of VPN providers offer a variety of options for VPN protocols, such as WireGuard or IPSec. Ultimately, choosing between IPSec and WireGuard depends on many factors, including connection speeds, compatibility with existing network infrastructure, and business or individual needs.

### **WireGuard VPN**

WireGuard is a high-speed VPN protocol, with advanced encryption, to protect users when they are accessing the internet. It’s designed to be simple to set up and maintain. WireGuard can be used for both site-to-site connection and client-server connections. WireGuard is relatively newer than IPSec, and is used by many people due to the fact that its download speed is enhanced by using fewer lines of code. WireGuard is also open source, which makes it easier for users to deploy and debug. This protocol is useful for processes that require faster download speeds, such as streaming video content or downloading large files.

### **IPSec VPN**

IPSec is another VPN protocol that may be used to set up VPNs. Most VPN providers use IPSec to encrypt and authenticate data packets in order to establish secure, encrypted connections. Since IPSec is one of the earlier VPN protocols, many operating systems support IPSec from VPN providers.

Although IPSec and WireGuard are both VPN protocols, IPSec is older and more complex than WireGuard. Some clients may prefer IPSec due to its longer history of use, extensive security testing, and widespread adoption. However, others may prefer WireGuard because of its potential for better performance and simpler configuration.

## **Key Takeaways**

A VPN protocol is similar to a network protocol: It’s a set of rules or instructions that will determine how data moves between endpoints. There are two types of VPNs: remote access and site-to-site. Remote access VPNs establish a connection between a personal device and a VPN server and encrypt or decrypt data exchanged with a personal device. Enterprises use site-to-site VPNs largely to extend their network to different locations and networks. IPSec can be used to create site-to-site connections and WireGuard can be used for both site-to-site and remote access connections.

TEST

![image.png](Google%20Networking%20Roadmap/image%2019.png)

![image.png](Google%20Networking%20Roadmap/image%2020.png)

![image.png](Google%20Networking%20Roadmap/image%2021.png)

### Module 3

#### **Introduction to network intrusion tactics**

![image.png](Google%20Networking%20Roadmap/image%2022.png)

Key terms

- Ping of death

a type of DoS attack that is caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64 kilobytes, the maximum size for a correctly formed ICMP packet.

- DOS

A denial of service attack is an attack that targets a network or server and floods it with network traffic.

- DDOS

A distributed denial of service attack, or DDoS, is a kind of DoS attack that uses multiple devices or servers in different locations to flood the target network with unwanted traffic.

Network level Dos attackd in banwidth

- SYN

A SYN flood attack is a type of DoS attack that simulates the TCP connection and floods the server with SYN packets.

Step_1, The first step in the handshake is for the device to send a SYN, or synchronize, request to the server.

Step_2,Then, the server responds with a SYN/ACK packet to acknowledge the receipt of the device's request and leaves a port open for the final step of the handshake.

Step_3,Once the server receives the final ACK packet from the device, a TCP connection is established.

attack idea - Malicious actors can take advantage of the protocol by flooding a server with SYN packet requests for the first part of the handshake.

- But if the number of SYN requests is larger than the number of available ports on the server, then the server will be overwhelmed and become unable to function.

- ICMP Flood
- An ICMP flood attack is a type of DoS attack performed by an attacker repeatedly sending ICMP packets to a network server.

ICMP stands for Internet Control Message Protocol.

CMP is an internet protocol used by devices to tell each other about data transmission errors across the network

![image.png](Google%20Networking%20Roadmap/image%2023.png)

# Read tcpdump logs

**0:38/4:04**

A **network protocol analyzer**, sometimes called a packet sniffer or a packet analyzer, is a tool designed to capture and analyze data traffic within a network. They are commonly used as investigative tools to monitor networks and identify suspicious activity. There are a wide variety of network protocol analyzers available, but some of the most common analyzers  include:

- SolarWinds NetFlow Traffic Analyzer
- ManageEngine OpManager
- Azure Network Watcher
- Wireshark
- tcpdump

This reading will focus exclusively on tcpdump, though you can apply what you learn here to many of the other network protocol analyzers you'll use as a cybersecurity analyst to defend against any network intrusions. In an upcoming activity, you’ll review a tcpdump data traffic log and identify a DoS attack to practice these skills.

## **tcpdump**

**tcpdump** is a command-line network protocol analyzer. It is popular, lightweight–meaning it uses little memory and has a low CPU usage–and uses the open-source libpcap library. tcpdump is text based, meaning all commands in tcpdump are executed in the terminal. It can also be installed on other Unix-based operating systems, such as macOS®. It is preinstalled on many Linux distributions.

tcpdump provides a brief packet analysis and converts key information about network traffic into formats easily read by humans. It prints information about each packet directly into your terminal. tcpdump also displays the source IP address, destination IP addresses, and the port numbers being used in the communications.

## **Interpreting output**

tcpdump prints the output of the command as the sniffed packets in the command line, and optionally to a log file, after a command is executed. The output of a packet capture contains many pieces of important information about the network traffic.

![types of information presented in a tcpdump packet capture.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/B-PaECh0ToSFgBWpFczYZg_4896abe8c06443f08eec4dc003dcf8f1_image.png?expiry=1786394062410&hmac=7yIkHIYseSAD7AdH3klvJWiIcmqFDOutmSBEnPORdiA)

Some information you receive from a packet capture includes:

- **Timestamp**: The output begins with the timestamp, formatted as hours, minutes, seconds, and fractions of a second.
- **Source IP**: The packet’s origin is provided by its source IP address.
- **Source port**: This port number is where the packet originated.
- **Destination IP**: The destination IP address is where the packet is being transmitted to.
- **Destination port**: This port number is where the packet is being transmitted to.

**Note:** By default, tcpdump will attempt to resolve host addresses to hostnames. It'll also replace port numbers with commonly associated services that use these ports.

## **Common uses**

tcpdump and other network protocol analyzers are commonly used to capture and view network communications and to collect statistics about the network, such as troubleshooting network performance issues. They can also be used to:

- Establish a baseline for network traffic patterns and network utilization metrics.
- Detect and identify malicious traffic
- Create customized alerts to send the right notifications when network issues or security threats arise.
- Locate unauthorized instant messaging (IM), traffic, or wireless access points.

However, attackers can also use network protocol analyzers maliciously to gain information about a specific network. For example, attackers can capture data packets that contain sensitive information, such as account usernames and passwords. As a cybersecurity analyst, It’s important to understand the purpose and uses of network protocol analyzers.

## **Key takeaways**

Network protocol analyzers, like tcpdump, are common tools that can be used to monitor network traffic patterns and investigate suspicious activity. tcpdump is a command-line network protocol analyzer that is compatible with Linux/Unix and macOS®. When you run a tcpdump command, the tool will output packet routing information, like the timestamp, source IP address and port number, and the destination IP address and port number. Unfortunately, attackers can also use network protocol analyzers to capture data packets that contain sensitive information, such as account usernames and passwords.

# Real-life DDoS attack

**0:16/4:05**

Previously, you were introduced to Denial of Service (DoS) attacks. You also learned that volumetric distributed DoS (DDoS) attacks overwhelm a network by sending unwanted data packets in such large quantities that the servers become unable to service normal users. This can be detrimental to an organization. When systems fail, organizations cannot meet their customers' needs. They often lose money, and in some cases, incur other losses. An organization’s reputation may also suffer if news of a successful DDoS attack reaches consumers, who then question the security of the organization.

In this reading you’ll learn about a 2016 DDoS attack against DNS servers that caused major outages at multiple organizations that have millions of daily users.

## **A DDoS targeting a widely used DNS server**

In previous videos, you learned about the function of a DNS server. As a review, DNS servers translate website domain names into the IP address of the system that contains the information for the website. For instance, if a user were to type in a website URL, a DNS server would translate that into a numeric IP address that directs network traffic to the location of the website’s server.

On the day of the DDoS attack we are studying, many large companies were using a DNS service provider. The service provider was hosting the DNS system for these companies. This meant that when internet users typed in the URL of the website they wanted to access, their devices would be directed to the right place. On October 21, 2016, the service provider was the victim of a DDoS attack.

## **Leading up to the attack**

Before the attack on the service provider, a group of university students created a botnet with the intention to attack various gaming servers and networks. A **botnet** is a collection of computers infected by malware that are under the control of a single threat actor, known as the “bot-herder." Each computer in the botnet can be remotely controlled to send a data packet to a target system. In a botnet attack, cyber criminals instruct all the bots on the botnet to send data packets to the target system at the same time, resulting in a DDoS attack.

The group of university students posted the code for the botnet online so that it would be accessible to thousands of internet users and authorities wouldn’t be able to trace the botnet back to the students. In doing so, they made it possible for other malicious actors to learn the code to the botnet and control it remotely. This included the cyber criminals who attacked the DNS service provider.

## **The day of attack**

At 7:00 a.m. on the day of the attack, the botnet sent tens of millions of DNS requests to the service provider. This overwhelmed the system and the DNS service shut down. This meant that all of the websites that used the service provider could not be reached. When users tried to access various websites that used the service provider, they were not directed to the website they typed in their browser. Outages for each web service occurred all over North America and Europe.

The service provider’s systems were restored after only two hours of downtime. Although the cyber criminals sent subsequent waves of botnet attacks, the DNS company was prepared and able to mitigate the impact.

## **Key takeaways**

As demonstrated in the above example, DDoS attacks can be very damaging to an organization. As a security analyst, it’s important to acknowledge the seriousness of such an attack so that you’re aware of opportunities to protect the network from them. If your network has important operations distributed across hosts that can be dynamically scaled, then operations can continue if the baseline host infrastructure goes offline. DDoS attacks are damaging, but there are concrete actions that security analysts can take to help protect their organizations. Keep going through this course and you will learn about common mitigation strategies to protect against DDoS attacks.