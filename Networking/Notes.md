# Notes 

## Intro to Networking 
Computer Network = Devices connected to each other to share resources. Enables communication between devices. 

LAN = Small and covers a limited network, e.g Home wifi. It allows devices to communicate with one another. 

WAN = Large, connects everyone world wide, e.g Internet. 

<img width="430" height="130" alt="image" src="https://github.com/user-attachments/assets/d61eb2a3-7453-46af-96d9-9240ae982293" />

## Switches, Routers and firewalls 

Switches = Connects devices within the same network, using Ethernet Cables. Manages dataflow within a LAN.

Router = Direct traffic between networks. Also, connects different networks, for e,g your home network with the internet. 

Firewalls = Protects from unauthorised access. Also, it monitors and controls incoming and outgoing traffic. 

## Ip Address & Mac Address

Ip address = Unique identifiers for devices. IPV4  and IPV 6 (longer). They enable devices to identify and communicate with each other on the network it can be the internet, or other networks. Assigned by Network

Mac address = Unique Idenfitifier assigned to a network device. (Laptop, Smartphone) Without them devices, wouldn't be able to communicate within their local network (KEY DIFFERENCE). When your router or switch wants to send information to a specific device (like your phone), it uses the MAC address to know exactly where to send it. Built into the hardware.

Your message (data) needs both:

The IP address to find the right location (routing).
The MAC address to deliver it to the correct device once it gets there.

## Ports & Protocals

Ports = logical endpoints for communication. For example, when your device wants to send or receive data, it uses these PORTS to ensure that the data goes into the right port (place)

Protocals = Defines how data is formatted and transmitted across a network. 

TCP is a PROTOCAL, that devices follow to communicate with one another. 
<img width="616" height="328" alt="image" src="https://github.com/user-attachments/assets/fe2f500a-0af2-4a5c-897b-4860e46c1bd9" />

UDP is another protocal. 
It doesn't need connection to allow data to be sent and received. However, this means that there is no guarantee that the data will reach its destination. 
<img width="470" height="257" alt="image" src="https://github.com/user-attachments/assets/ed7c605a-8c99-4b11-a209-09270d64df9e" />

TCP V UDP 
<img width="494" height="262" alt="image" src="https://github.com/user-attachments/assets/3dbf6eb0-f706-4128-843a-7d12dfcd2d45" />


## OSI Model - How Data Travels between devices

OSI Model = Framework that helps us understand how data mmoves through a network. 

Why do we need a communication model ?
1. Applications can be built regardless of the network (Ethernet, WIFI). Without a model, applications would have to be built taking into account the type of network.
2. Easier to upgrade network.
3. Innovation/Updates can happen to each level of the model without affecting the whole system.

7 Layers 
<img width="418" height="286" alt="image" src="https://github.com/user-attachments/assets/3f378218-9da0-4f10-af74-3d2656d60622" />

1. Physical - Transfers raw bit streams (small pieces of data) over a physical medium (wifi, cables)
2. Data Link - Provides node to node data transfer, corrects errors in the physical layer. Ensures data is correctly transferred between nodes (Mac Addresses, switches and bridges).
3. Network - Determines how packets are sent to the recipient. Decides the best path for data to pass through different networks (IP Addresses, Routers).
4. Transport - Delivers reliable data transfers to the upper layers. Ensures data parcels arrive safely and in sequence. (TCP, UDP).
5. Session - Establishes, maintains and terminates connections (Session Management Protocols). 
6. Presentation - Translates data between application layer and network (Handles - Encryption, Data Formatting) 
7. Application - Provides network services directly to the application. The layer you actually see and use, like your web browser. (HTTP, FTP, SMTP)

TCP/IP Layer
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c0881853-60cc-4ce8-bb43-afa06526833c" />

1. Application Layer - Where network services are directly provided to the application (HTTP, etc) 
2. Transport Layer - Where End to End communication happens (TCP, UDP)
3. Internet Layer - Logical addressing and routing data across different networks (IP)
4. Network access Layer - (Same as L1 and L2 of OSI). Physical and datalink aspects (Physical, Wireless, and Lan). How is it the same as L1 and L2  --> Physically sends data (electrical signals, light, radio waves). Uses MAC addresses to deliver data to the right device on a local network.

OSI Layers; POV of Sender 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/88a02a2b-397a-4425-a660-0e0e3d51698a" />

Pov of Receiver
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6809ba10-4c8c-4dcf-afc2-6798ec943c0f" />


