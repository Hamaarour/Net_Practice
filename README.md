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
Also a device with multiple ports that accepts Ethernet connections from network devices but Unlike a hub a switch is intelligent . a switch can actually learn the physical adresses of the devices that are connected to it and it stores these physical adresses called Mac adresses in its table 
<img src="" width="200" height="150" />
LINK => [What is a Switch/Hub/Router](https://www.youtube.com/watch?v=1z0ULvg_pW8&t=141s&ab_channel=PowerCertAnimatedVideos)

### In Summary

Hubs and SWitches used to exchange data between devices on a computer network. A hub contains multiple ports. When a packet arrives at one port, it is copied to the other ports so that all segments of the LAN can see all packets, Switch is a device that filters and forwards packets between LAN segments. Switches operate at the data link layer (layer 2) and sometimes the network layer (layer 3) of the OSI Reference Model and therefore support any packet protocol. LANs that use switches to join segments are called switched LANs or, in the case of Ethernet networks, switched Ethernet LANs.

Hub and switches is used to exchanges data whitin a local area network (Lan), Not used to exchange data outside of the local area network (Lan) to the internet.

To exchange data outside your network a device needs to be able to read IP adresses and that's where a router comes in.

## Router

A router is a networking device that forwards data packets between computer networks. Routers perform the traffic directing functions on the Internet. Data sent through the internet, such as a web page or email, is in the form of data packets. A packet is typically forwarded from one router to another router through the networks that constitute an internetwork (e.g. the Internet) until it reaches its destination node.