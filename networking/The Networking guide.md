
>This page contains the contents about networking, this may include theory, programs and real world applications

## So let's get started

### What is a computer network ?

A set of nodes connected by a communication medium. Where these nodes can be any device which can send and receive data such as printers, computer etc.
And the link can be any medium which can transport the signals such as wires, cables, air optical cables etc

In short, computer network can be said as the collection of interconnected of computers which can share **data** as well as **resources**. Communication can be said as the process of **exchanging information** between two devices or persons

## Uses of computer networks

BUSINESS USES 
- for sharing information
- for sharing resources (people in office sharing a common printer)
HOME USES
- Person to person communication
- interactive entertainment (TV, online games)
- E-commerce (online shopping)
And also in many other fields


## Network topologies 

Network topologies are basically the pattern in which the nodes are arranged in the network that is the way in which computers are connected

Mainly there are 5 network topologies
- [Bus topology](#Bus-topology)
- [Ring topology](#Ring-topology)
- [Star topology](#Star-topology)
- [Mesh topology](#Mesh-topology)
- [Hybrid topology](#Hybrid-topology)

## Bus-topology

- Simplest topology
- All computers are connected through a single cable called the backbone
- Limited failure, moderate data speed and low cost are some plus points .
- reconfiguration is difficult, signal interference and extensive cabling are some disadvantages

## Ring-topology

- All computers are connected in a ring format, that is closed loop
- Each node connects exactly to two nodes.
- The failure of one computer results in the failure of the entire network

## Star-topology

- The computers are connected to single hub in this network
- This hub is the center node and all the others are connected to this node
-  the failure of this device can cause the entire network to fail

## Mesh-topology

- All nodes are interconnected here, That is a single node has a connection to every other node (  not in every case)
- Failure of one system does  not affect in the working of others
- Internet is an example of mesh topology
- There are two types - fully connected (every node to other every node) and partial 

## Hybrid-topology

- Combination of every other topologies
- two or more topologies are combined together
- reliable, flexible and effective are some advantages
- high cost and high maintenance are some disadvantages

## Network Hardware

### Types of Network based on area covered



## **Internet work or The Internet**

- It is a collection of interconnected networks. An internet is formed when distinct networks are interconnected.
- Improved availability and improved reach are some perks of internet

## Transmission Modes

Communication between two devices can be

- [Simple](#Simple)
- [Full-duplex](#Full-duplex)
- [Half-duplex](#Half-duplex)

![[Pasted image 20231015232257.png]]

### Simple
### Half-duplex

### Full-duplex


## Network Software

### Protocol

In a computer networks, communication occurs between two entities in different systems. The entity is capable of sending and receiving data . But two entities cannot send bit streams of data to each other and claims to understand that. So for communication to occur, the both entities must agree to a protocol.

A **protocol** is basically a set of rules that govern data communication. A protocol defines what it is communicated, when it is communicated and how it is communicated

The key elements of a protocol are
- syntax - format or structure of data blocks
- semantics - this is the section which defines the meaning of each section of the data bits . That is how is a specified pattern should be interpreted and what action should be taken based on that interpretation
- Timing - when data and how much speed the data should be sent

### Protocol Hierarchy - Layered structure


To reduce the complexity in design, the networks are arranged as a stack of layers. Each layer performs separate functions and provide services to the upper layers. The number of layers, the name of layers and the functions of layers differ from network to network.
In a layer n architecture, layer n of one machine carries on conversation with the n layer of the other machine and the rules used in this conversation are collectively called the n layer protocol.

![[Pasted image 20231016065915.png]]
*credits : geeks for geeks*

The above figure is an example for 5 layered architecture . 