>This page covers about the network layer


>From a DevOps engineer's perspective, several networking concepts are particularly relevant:

1. **Routing Algorithms:** Understanding routing algorithms like Shortest Path Routing, Distance Vector Routing, and Link State Routing is beneficial. While DevOps engineers might not be directly configuring routers or implementing these algorithms, having a grasp of how routing works aids troubleshooting network issues and optimizing application performance.
    
2. **Quality of Service (QoS):** DevOps engineers need to ensure applications and services meet certain performance levels. Understanding QoS requirements and techniques for achieving good QoS helps in managing network resources effectively to meet application demands.
    
3. **Congestion Control Algorithms:** DevOps involves monitoring and optimizing system performance. Awareness of congestion control algorithms aids in identifying and addressing network bottlenecks, ensuring smooth operations for applications and services.
    

While concepts like Multicast Routing or Routing for Mobile Hosts might be less directly applicable to typical DevOps tasks, a general understanding of these topics can still offer a broader perspective on network design and behavior, aiding in troubleshooting and optimizing overall system performance.


### What is a network layer 

The network layer, also known as Layer 3 in the OSI (Open Systems Interconnection) model or the Internet Protocol Suite, is a crucial part of networking. It is responsible for the source to destination (end to end) transfer of packets across multiple network links.
Routers and gateways are present in this layer, that is, the routing to the final destination happens in this layer. And also this layer takes care about selecting the route so that it does not overload the network

### What are the routers ?

Routers are network layer  devices which helps to connect two or more networks. They basically pass the packets to the destination by looking up on the routing table. Each router has a routing table. Whenever a new packet arrives, it looks at the routing table. The routing table consists of mainly three fields :
- The network ID : it's basically the destination ID
- Cost : It is the cost or metric through which the packet has to move through to reach its final destination
- Next Hop : Also known as the gateways, it is the address of the next station which the packet has to move 

## Routing Algorithms

Routing is the process of sending a packet from the source to the destination. So during the flow of the packets from the sender to the receiver, it is really necessary to find the most feasible path for packets to travel. Routing algorithm does exactly this, that is, these algorithms help us to calculate these paths for packets to travel.

Two types of routing algorithm :
1. Non-adaptive (Static routing)
2. Adaptive (Dynamic routing)


