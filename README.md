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



