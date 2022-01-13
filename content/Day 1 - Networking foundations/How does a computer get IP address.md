---
title: "How does a computer gets and IP address?"
draft: false
weight: 55
pre: 
---


**Static vs Dynamic**
---
How does your computer get its IP address? An IP address can be either dynamic or static.

<img src='/images/dynamic_vs_static.png' width='600px'>

**Static** address is one that you configure yourself by editing your computer’s network settings. This type of address is rare, and it can create network issues if you use it without a good understanding of TCP/IP.

**Dynamic** addresses are the most common. They’re assigned by the Dynamic Host Configuration Protocol (DHCP), a service running on the network. DHCP typically runs on network hardware such as routers or dedicated DHCP servers. Dynamic IP addresses are issued using a leasing system, meaning that the IP address is only active for a limited time. If the lease expires, the computer will automatically request a new lease.

Please re-visit the [DHCP section](dnsdhcp.html#dynamic-host-configuration-protocol-dhcp) if you need a refresh on how DHCP works.

If you have a Windows machine, you also might want to familiarize yourself on how you can configure static or dynamic (DHCP) IP configuration.

***Windows Static IP Configuration:***
<img src='/images/static_ip_config.png' width='600px'>

***Windows Dynamic IP (DHCP) Configuration:***
<img src='/images/dynamic_ip_config.png' width='600px'>