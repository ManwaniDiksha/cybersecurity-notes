# OSI Model
- Open Systems Interconnection Reference Model.
- Used to describe a broad overview of how data traverses our systems.
- OSI can be applied to many different protocols. Many protocols might operate at an individual layer of the OSI model.

# Layers of the OSI Model

| Layer | Name         | Mnemonic |
|------|-------------|----------|
| 7    | Application  | All      |
| 6    | Presentation | People   |
| 5    | Session      | Seem     |
| 4    | Transport    | To       |
| 3    | Network      | Need     |
| 2    | Data Link    | Data     |
| 1    | Physical     | Processing |

## Layer 1 - Physical Layer 
- Describes the physical signals that we send through the cables on our network
- This layer isn't about protocols.
- Cable related problems would be considered as a physical layer problem.
- Troubleshooting includes fixing your cabling, running loopback tests, testing/replacing cables, swapping adapter cards, etc.

## Layer 2 - Data Link Layer
- Fundamental layer used to communicate between two devices on the network.
- Also referred to as the MAC(Media Access Control) address layer / DLC(Data Link Control) layer. Commonly associated with the network cards that are in our devices. 
- Physical Address of device = Data link control address/MAC address. 
- Also referred to as the "switching" layer because the network switches that we use on our network determine how to forward traffic based on the destination MAC address. 

## Layer 3 - Network Layer
- Also referred to as the "routing" layer because this is the layer that routers use to determine how to forward traffic based on the destination IP(Internet Protocol) address.
- Fragments frames to traverse different networks.

## Layer 4 - Transport Layer
- We're referring to the ability to transport information from one device to another.
- Also referred to as the "post office" layer since it is responsible for getting your information from one side of the network to the other. 
- Protocols that are often used and operate at layer 4 are TCP(Transmission Control Protocol) and UDP(User Datagram Protocol).
- These protocols are responsible for getting all of the information within our IP packets from one device to another.

## Layer 5 - Session Layer
- Provides communication management between point A and point B.
- Responsible for anything related to initiating a session, stopping a session, restarting a session. 
- Using a control protocol or tunneling information within existing data is done using layer 5.

## Layer 6 - Presentation Layer
- Responsible for putting all the data in a format that will be eventually seen by human eyes.
- This refers to character encoding, application encryption & decryption.
- Often combined with the Application Layer.

## Layer 7 - Application Layer
- The Top Layer.
- This is the layer that we see on our screen. 
- Anytime we are interacting with an application we are operating at layer 7.
- Common protocols that would operate at OSI layer 7 are HTTP & HTTPS, FTP, DNS, POP3, and many more other application protocols. 

# Real-world to OSI model
| Layer | Name         | Examples/Concepts |
|-------|--------------|-------------------------------|
| 7    | Application  | UI      |
| 6    | Presentation | Application encryption(SSL/TLS)   |
| 5    | Session      | Control protocols, tunneling protocols     |
| 4    | Transport    | TCP segment, UDP datagram       |
| 3    | Network      | IP Address, Router, Packet  |
| 2    | Data Link    | Frame, MAC address, Extended Unique Identifier(EUI-48, EUI-64), Switch |
| 1    | Physical     | Cables, fiber, and the signal itself |