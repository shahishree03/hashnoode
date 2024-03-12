---
title: "Routers"
datePublished: Sat May 06 2023 17:36:51 GMT+0000 (Coordinated Universal Time)
cuid: clhc9ora0000c09mkgw9cd653
slug: routers
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1683392976765/9377e24c-f6d3-4f6a-8b25-4e6574be0f88.jpeg
tags: routing, internet, networking

---

In computer networking, a router is a device that forwards data packets between computer networks. A router connects multiple devices or networks and manages the traffic between them.

Routers operate at the network layer (layer 3) of the OSI model and use routing tables to determine the best path for data to take across a network. They typically connect two or more networks, such as a home network and the internet, and are responsible for routing data between them.

Routers can also perform other functions, such as acting as a firewall to protect a network from unauthorized access or providing Network Address Translation (NAT) to allow multiple devices to share a single internet connection.

Common types of routers include home routers, enterprise routers, and service provider routers. Home routers are typically smaller and designed for use in a household or small office, while enterprise routers are more powerful and designed for use in more extensive networks. Internet service providers use service provider routers to connect their customers to the internet.

## **Use of Routers**

Routers have several important uses in computer networking. Here are some of the main ways that routers are used:

**Connecting multiple networks:** Routers are used to connect multiple networks, such as a home network and the internet, or different networks within an organization. By forwarding data packets between networks, routers enable communication between devices on different networks.

**Routing traffic:** Routers use routing tables to determine the best path for data to take across a network. This helps to ensure that data is delivered efficiently and reliably to its destination.

**Providing network security:** Routers can be used to provide network security, by acting as a firewall to block unauthorized access to a network. They can also be used to create virtual private networks (VPNs) to allow secure remote access to a network.

**Managing bandwidth:** Routers can be used to manage bandwidth, by prioritizing certain types of traffic over others. For example, a router can be configured to prioritize video streaming traffic over email traffic, to ensure a better viewing experience.

**Sharing Internet access**: Routers can be used to share a single internet connection among multiple devices, by using Network Address Translation (NAT) to assign unique IP addresses to each device on a local network.

Overall, routers are a critical component of modern computer networks and are essential for enabling communication and ensuring the efficient and secure transmission of data.

## **Types of Routers**

There are several different types of routers, each with its own specific features and capabilities. Here are some of the most common types of routers:

1. **Home routers:** Home routers are designed for use in small home or office networks, and typically have four to eight Ethernet ports for connecting devices. They often include built-in wireless access points and are designed to be easy to set up and use.
    
2. **Wireless routers**: Wireless routers are a type of home router that includes a built-in wireless access point, allowing devices to connect to the network using Wi-Fi. They are commonly used in homes, cafes, and other public spaces where users need wireless connectivity.
    
3. **Edge routers:** Edge routers are used in service provider networks to connect customer networks to the internet. They are designed to handle large volumes of traffic and to support advanced routing protocols, such as Border Gateway Protocol (BGP).
    
4. **Core routers:** Core routers are used in large enterprise or service provider networks to connect multiple edge routers. They are designed to handle high volumes of traffic and to provide fast and reliable routing.
    
5. **Virtual routers:** Virtual routers are software-based routers that run on virtual machines or cloud platforms. They are often used in virtualized data centres or cloud environments to provide routing between virtual machines or between on-premises and cloud-based resources.
    
6. **Peering routers:** Peering routers are used by internet service providers to connect their networks. They are designed to handle large volumes of traffic and to support peering agreements between providers.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683394172504/4fd273c9-9955-49f4-81d7-37a8a6a95595.jpeg align="center")

Overall, routers are an essential component of modern computer networks, and the specific type of router needed depends on the size and complexity of the network being used.

## Routing

Routing is the process of selecting the best path for network traffic to take from a source device to a destination device across a computer network. Routers are responsible for performing routing in computer networks.

When a device on a network wants to send data to another device on a different network, it sends the data packet to the router that is connected to its own network. The router then uses its routing table to determine the best path for the data to take to reach its destination.

It also helps to ensure that data is delivered efficiently and reliably to its destination, even in the presence of network failures or congestion.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683394531575/f99848ab-b31b-4ee9-b130-46f684066862.png align="center")

## Routing Protocols

Routing protocols specify a way for the router to identify other routers on the network and make dynamic decisions to send all network messages. There are several protocols, which are given below:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1683394560207/2c4ee7eb-7e2a-4075-b4f2-f1016bfbbd2a.png align="center")

**Open Shortest Path First (OSPF):** It is used to calculate the best route for the given packets to reach the destination, as they move via a set of connected networks. It is identified by the Internet Engineering Task Force **(IETF)** as Interior Gateway Protocol.

**Border Gateway Protocol (BGP):** It helps manage how packets are routed on the internet via the exchange of information between edge routers. It provides network stability for routers if one internet connection goes down while forwarding the packets, it can adapt to another network connection quickly to send the packets.

**Interior Gateway Routing Protocol (IGRP):** It specifies how routing information will be exchanged between gateways within an independent network. Then, the other network protocols can use the routing information to determine how transmissions should be routed.

**Enhanced Interior Gateway Routing Protocol (EIGRP):** In this protocol, if a router is unable to find a path to a destination from the tables, it asks route to its neighbors, and they pass the query to their neighbors until a router has found the path. When the entry of the routing table changes in one of the routers, it informs its neighbors only about the changes but does not send the entire table.

**Exterior Gateway Protocol (EGP):** It decides how routing information can be exchanged between two neighbor gateway hosts, each of which has its own router. Additionally, it is commonly used to exchange routing table information between hosts on the internet.

**Routing Information Protocol (RIP):** It determines how routers can share information while transferring traffic among the connected group of local area networks. The maximum number of hops that can be allowed for RIP is 15, which restricts the size of networks that RIP can support.