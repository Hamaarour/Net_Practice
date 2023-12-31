# Net_Practice
You will have to configure small-scale networks. To do so, it will be necessary to understand how TCP/IP addressing works.

## What is a network switch?

A network switch connects devices within a network (often a local area network, or LAN*) and forwards data packets to and from those devices. Unlike a router, a switch only sends data to the single device it is intended for (which may be another switch, a router, or a user's computer), not to networks of multiple devices.

<p align="center">
    <img src="https://cf-assets.www.cloudflare.com/slt3lc6tev37/6ENfwtM3iUH99JpYoEC9FY/04abc1654ceff2645f50713394ebcb73/network-switch.svg" width='900px' height='600px'>
</p>
*(A local area network (LAN) is a group of connected devices within close physical proximity. Home WiFi networks are one common example of a LAN.)

## What is the purpose of a Hub
the porpose is to connect all of your network devices toghether on an internal network, it's devices that has a multiple ports that accepts Ethernet connections from network devices
the only thing a hub knows is when a device is connected to one of its ports.

## What is a Switch
Also a device with multiple ports that accepts Ethernet connections from network devices but Unlike a hub a switch is intelligent . a switch can actually learn the physical adresses of the devices that are connected to it and it stores these physical adresses called Mac adresses in its table.
<br>
<img src="https://github.com/Hamaarour/Net_Practice/blob/main/assets/S_H_R.gif" width="100%" height="400" />
LINK => [What is a Switch/Hub/Router](https://www.youtube.com/watch?v=1z0ULvg_pW8&t=141s&ab_channel=PowerCertAnimatedVideos)

### In Summary

Hubs and SWitches used to exchange data between devices on a computer network. A hub contains multiple ports. When a packet arrives at one port, it is copied to the other ports so that all segments of the LAN can see all packets, Switch is a device that filters and forwards packets between LAN segments. Switches operate at the data link layer (layer 2) and sometimes the network layer (layer 3) of the OSI Reference Model and therefore support any packet protocol. LANs that use switches to join segments are called switched LANs or, in the case of Ethernet networks, switched Ethernet LANs.

Hub and switches is used to exchanges data whitin a local area network (Lan), Not used to exchange data outside of the local area network (Lan) to the internet.

To exchange data outside your network a device needs to be able to read IP adresses and that's where a router comes in.

## Router

A router is a networking device that forwards data packets between computer networks. Routers perform the traffic directing functions on the Internet. Data sent through the internet, such as a web page or email, is in the form of data packets. A packet is typically forwarded from one router to another router through the networks that constitute an internetwork (e.g. the Internet) until it reaches its destination node.

<p align="center">
    <img src="" width='900px' height='600px'>
</p>

## What is a Gateway

A gateway is a piece of networking hardware used in telecommunications for telecommunications networks that allows data to flow from one discrete network to another. Gateways are distinct from routers or switches in that they communicate using more than one protocol to connect a bunch of networks and can operate at any of the seven layers of the open systems interconnection model (OSI).

### How Router work ?

Think of a router as an air traffic controller and data packets as aircraft headed to different airports (or networks). Just as each plane has a unique destination and follows a unique route, each packet needs to be guided to its destination as efficiently as possible. In the same way that an air traffic controller ensures that planes reach their destinations without getting lost or suffering a major disruption along the way, a router helps direct data packets to their destination IP address.

In order to direct packets effectively, a router uses an internal routing table — a list of paths to various network destinations. The router reads a packet's header to determine where it is going, then consults the routing table to figure out the most efficient path to that destination. It then forwards the packet to the next network in the path.


### IP Address 

An Internet Protocol address (IP address) is a numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication. An IP address serves two main functions: host or network interface identification and location addressing.

### what is a subnetting
Subnetting is the process of creating a subnetwork (also known as a subnet) within a network. Network interfaces and devices within a subnet can communicate with each other directly. Routers facilitate communication between different subnets.
Taking a network and dividing it into a sub-networks, called subnets. This is done to take a large network and break it down into smaller networks, to improve performance and security.

## Seven attributes of a Subnet Mask

1- Network ID => 
2- Broadcast ID =>
3- First Host IP =>
4-  Last Host IP =>
5- Next Network =>
6-  IP Address =>
7- Number of IP Addresses in a Sub-Network =>
8- CIDR/Subnet => 


HOST ==> are any device which send or recive traffic
IP   ==>  is the identity of each host
=======
SPEED TESTS:
============
Speed Tip #1 : 
Group Size can be easily multiplied by 10. Then doubled or tripled, as necessary 
Speed Tip #2 : 
Every Group Size lands on 128 at some point. 
Speed Tip #3 : 
Every group size lands on the Subnet value of the same column, and every column to the LEFT. 
Speed Tip #4 : 
Start higher, and subtract. 


Types of casting :

1- Unicast
    *one to one* send data to a single device on a network by Mac address or IP address
2- Multicast
    *one to many* send data to a group of devices on a network by Mac address or IP address
3- Broadcast
    *one to all* send data to all devices on a network by Mac address or IP address
        *limited brodcast* 
# TCP
TCP stands for Transmission Control Protocol a communications standard that enables application programs and computing devices to exchange messages over a network. It is designed to send packets across the internet and ensure the successful delivery of data and messages over networks.

TCP organizes data so that it can be transmitted between a server and a client. It guarantees the integrity of the data being communicated over a network. Before it transmits data, TCP establishes a connection between a source and its destination, which it ensures remains live until communication begins. It then breaks large amounts of data into smaller packets, while ensuring data integrity is in place throughout the process, toensures end-to-end data delivery without loss any of data.

HOW send data : As we know in TCP protocol, for the first time, it tries to sent one packet to the destination, and check if the packet is well received by ensuring the connection remains live. Each time, it adds a packet to be sent, meaning that for the second time, it sends the double of packets sent before, and checks if the connection remains good. For the third time, it adds the double of the previous number of packets of the previous one, until a problem occurred in this connection. At this moment, it goes back the previous number of packets sent in order to keep this connection for an end-to-end data delivery of data, to Increase the transmitter speed and maintain accuracy. We can clarify this process with a simple mathematical formulate, which is: 2^(n). Where n is the number of times to send the packet in this connection correctly.

As a result, high-level protocols that need to transmit data all use TCP Protocol.Examples include peer-to-peer sharing methods like File Transfer Protocol (FTP), Secure Shell (SSH)...

# SUBNET MASK

A subnet mask is a 32 bits (4 bytes) address used to distinguish between a network address and a host address in the IP address. It defines the range of IP addresses that can be used within a network or a subnet.

# Routing Table

A routing table is a data table stored in a router or a network host that lists the routes to particular network destinations. In NetPractice, the routing table consists of 2 elements:

Destination: The destination specifies a network address on which a host is the end target of the packets. The route of default or 0.0.0.0/0, is the route that takes effect when no other route is available for an IP destination address. The default route will use the next-hop address to send the packets on their way without giving a specific destination. The default route will match any network.

Next hop: The next hop refers to the next closest router a packet can go through. It is the IP address of the next router on the packet's way. Every single router maintains its routing table with a next hop address.

