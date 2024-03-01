#### What is networking ??
Networking is basically a collection of devices which are connected together buy some medium such as Wi-Fi or Ethernet cables etc. in one physical location with the purpose to share resources and information with each other. They can communicate with the help of IP (Internet protocol) address and each device has some unique IP.


#### IP address

`172.16.0.0 ` This is an example of an IP address. It is a 32 bit value. IP addresses can range from `0.0.0.0 `to `255.255.255.255`. Each bit is an octet. And these IP addressees are divided into many classes such as A, B, C, D and E.

1. **Class A (1.0.0.0 to 126.255.255.255):**
    
    - The first octet is reserved for network identification, and the remaining three octets are for host addresses.
    - Supports a large number of networks with a relatively small number of hosts per network.
    - Example: 10.0.0.1, 126.255.255.255
2. **Class B (128.0.0.0 to 191.255.255.255):**
    
    - The first two octets are reserved for network identification, and the remaining two octets are for host addresses.
    - Suitable for medium-sized networks with a moderate number of hosts.
    - Example: 172.16.0.1, 191.255.255.255
3. **Class C (192.0.0.0 to 223.255.255.255):**
    
    - The first three octets are reserved for network identification, and the last octet is for host addresses.
    - Ideal for smaller networks with a limited number of hosts.
    - Example: 192.168.0.1, 223.255.255.255
4. **Class D (224.0.0.0 to 239.255.255.255):**
    
    - Reserved for multicast groups, used for multicasting data to multiple devices.
    - Not commonly used for host addressing.
5. **Class E (240.0.0.0 to 255.255.255.255):**

    - Reserved for experimental purposes and not intended for general use.

#### How devices talk to each other ??

In the case of LAN (Local area network) a device known as Switch helps in the communication. It sits within the LAN, and it facilitates the connection between all the devices within the LAN

Ok, so what if we want to talk to a server which is outside of LAN ? Here we use a device called router. It sits between LAN and outside networks (WAN) (Wide area networks). So a router connects devices on LAN and WAN. And the IP of the router is called a Gateway .

#### How to know whether the other device is inside or outside the LAN?


