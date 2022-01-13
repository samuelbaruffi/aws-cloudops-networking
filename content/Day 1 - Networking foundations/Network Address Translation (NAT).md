---
title: "Network Address Trasnlation (NAT)"
draft: false
weight: 47
pre: 
---


**Network Address Translation (NAT)**
---

**What Is NAT?**

NAT stands for network address translation. It’s a way to map multiple local private addresses to a public one before transferring the information. Organizations that want multiple devices to employ a single IP address use NAT, as do most home routers.

<img src='/images/nat.webp' width='900px'>
 

**How Does NAT Work?**

Let’s say that there is a laptop connected to a home router. Someone uses the laptop to search for directions to their favorite restaurant. The laptop sends this request in a packet to the router, which passes it along to the web. But first, the router changes the outgoing IP address from a private local address to a public address.

If the packet keeps a private address, the receiving server won’t know where to send the information back to — this is akin to sending physical mail and requesting return service but providing a return address of anonymous. By using NAT, the information will make it back to the laptop using the router’s public address, not the laptop’s private one.
 

**What is the Purpose of Network Address Translation?**

To communicate with the internet, a networking system requires a unique IP address. This 32-bit number identifies and locates the network device so a user can communicate with it.

The IPV4 addressing scheme of past decades technically made billions of these unique addresses available, but not all could be assigned to devices for communication. Instead, some were exempted and used for testing, broadcast, and certain reserved military purposes. While that left over 3 billion for communication, the proliferation of the internet has meant the addresses were near exhaustion.

The IPv6 addressing scheme was introduced as the solution to this weakness in the IPv4 addressing scheme. IPv6 recreates the addressing system so there are more options for allocating addresses, but it has taken several years to alter the networking system infrastructure and to implement. NAT was introduced by Cisco in the meantime and widely deployed.
 

**How Network Address Translation Works**

Network address translation permits a single device, such as a NAT firewall or NAT router or other network address translation device, to act as an agent between the public network and private networks—the internet and any local networks. This allows an entire group of devices to be represented by a single unique IP address when they do anything outside their network.

NAT works like a large company’s receptionist, with specific instructions on which calls and visitors to keep out, make wait, or send through, and where they should go. For example, you can tell the receptionist not to forward any visitors or calls without your request until you’re waiting for something specific; you can then leave instructions about letting that particular client communication through.

The client calls the company’s main number, because that public-facing number is the only one anyone knows. They tell the receptionist they need to speak with you, and the receptionist a) checks the instructions and knows you want the call forwarded, and b) matches your extension with a list to send the information to the right place. The caller never gets your private line.

Network address translation works similarly. The request arrives at the public IP address and port, and the NAT instructions send it where it should go without revealing the private IP addresses of the destinations.

**Advantages of Network Address Translation**

**Address conservation:** NAT conserves IP addresses that are legally registered and prevents their depletion.

**Network address translation security:** NAT offers the ability to access the internet with more security and privacy by hiding the device IP address from the public network, even when sending and receiving traffic. NAT rate-limiting allows users to limit the maximum number of concurrent NAT operations on a router and rate limit the number of NAT translations. This provides more control over the use of NAT addresses, but can also be used to limit the effects of worms, viruses, and denial-of-service (DoS) attacks. Dynamic NAT implementation creates a firewall between the internal network and the internet automatically. Some NAT routers offer traffic logging and filtering.

**Flexibility:** NAT provides flexibility; for example, it can be deployed in a public wireless LAN environment. Inbound mapping or static NAT allows external devices to initiate connections to computers on the stub domain in some cases.

**Simplicity:** Eliminates the need to renumber addresses when a network changes or merges.
Network address translation allows you to create an inside network virtual host to coordinate TCP load-balancing for internal network servers.

**Speed:** Compared to proxy servers, NAT is transparent to both destination and source computers, allowing for quicker direct dealing. In addition, proxy servers typically work at the transport layer or layer 4 of the OSI Reference Model or higher, making them slower than network address translation, which is a network layer or layer 3 protocol.

**Scalability:** NAT and dynamic host configuration protocol (DHCP) work well together, with the DHCP server doling out unregistered IP addresses for the stub domain from the list as necessary. Scaling up is easier, since you can increase the available range of IP addresses the DHCP configures to make room for additional network computers immediately instead of requesting more IP addresses from IANA as needs increase.

**Multi-homing:** Multiple connections to the internet, called multi-homing, helps maintain a reliable connection and reduces the chance of a shutdown in case of a failed connection. This also enables load-balancing via reducing the number of computers using any single connection. Multi-homed networks often connect to multiple ISPs, each assigning a range of IP addresses or a single IP address to the organization. Routers use network address translation to route between networks using different network address translation protocols. In a multi-homed network, the router uses part of the TCP/IP protocol suite, the border gateway protocol (BGP), to communicate; the stub domain side uses internal BGP or IBGP, and routers communicate with each other using external BGP or EBGP. Multi-homing reroutes all data through another router should one of the connections to an ISP fail.



