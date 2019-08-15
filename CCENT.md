# Cisco CCENT/CCNA ICND1 100-101

#### Chapter 1: The TCP/IP and OSI Networking Models
```
Two networking models: TCP/IP and OSI
Digital Subscriber Line (DSL)
Enterprise Network
Small Office Home Office (SOHO)
Protocol is a set of logical rules that devices must follow to communicate

Transmission Control Protocol (TCP), Layer 4
Internet Protocol (IP), Layer 3
International Business Machines (IBM)
IBM Systems Network Architecture (SNA), 1974, Layer 3
Synchronous Data Link Control (SDLC), Layer 2
International Standards Organization (ISO) - origin of OSI model
Open Systems Interconnection (OSI)
U.S. Department of Defense (DoD) - origin of TCP/IP model (RFC 1122)
Request for Comments (RFC)
Institute of Electrical and Electronic Engineers (IEEE)
Hypertext Transfer Protocol (HTTP), Tim Berners-Lee
User Datagram Protocol (UDP), Layer 4
Dotted-Decimal Notation (DDN), e.g. 192.168.43.1
Point to Point (PPP) and Frame Releay, Layer 2

Frame, Layer 2
Packet, Layer 3 
Segment or Datagram, Layer 4

Lan Hub, Layer 1, copies signals to all ports (also repeaters, cables)
Lan Switch, Layer 2 Switch, copies frames (also WAP, modems)
Router, Layer 3, reframes packets

Layering benefits: Less complex, standard interfaces, easier to learn, easier to develop, multivendor interoperability, modular engineering
```
#### Chapter 2: 
```
Enterprise network types: local-area network (LAN), wide-area network (WAN)
Two types of LAN: Ethernet LAN and Wireless LAN
Ethernet is a family of LAN standards defined by IEEE.
An Ethernet LAN switch provides physical ports for Ethernet cable connections.
One or more switch ports may connect to a Router providing Internet connection.
Wireless devices connect to an Ethernet network through a wireless LAN access point (AP).
On a SOHO network, a single device, a wireless router, might combine switch, AP and router functions.
Several switches may be connected to a distribution switch (SWD) which connects to a router.

10 Mbps    Ethernet          10BASE-T     802.3    Copper  100m
100 Mbps   Fast Ethernet     100BASE-T    802.3u   Copper  100m
1000 Mbps  Gigabit Ethernet  1000BASE-LX  802.3z   Fiber   5000m
1000 Mbps  Gigabit Ethernet  1000BASE-T   802.3ab  Copper  100m
10 Gbps    10 Gig Ethernet   10GBASE-T    802.3an  Copper  100m

Unshielded Twisted Pair (UTP)
Shielded Twisted Pair (STP)
Transmit or Receive over a PAIR of wires
Twisting reduced electromagnetic interference (EMI)

RJ-45 standard port and connector - up to 8 wires (four pairs)
10 Mbps and 100 Mbps standards use two pairs - one transmit pair, one receive pair.
1000BASE-T uses four pairs.

Network Interface Card (NIC) on computing device
RJ-45 Ethernet Port on Hub, Switch, wireless router.
Some switches may provide swappable/removable interfaces - small form factor pluggables (SFP)

Straight-through connections - same-pin connections, e.g. pin 1 to pin 1, pin 2 to pin 2, etc.
Crossover connections - pin 1 to pin 3, pin 2 to pin 6 and vice-versa
PC NICs, Routers, WAP transmit on pins 1,2
Hubs, Switches transmit on pins 3,6
Some switches support auto-mdix that detect incorrect cable wiring and adjust
1000Base-T adds pairs on pins 4,5 and 7,8

Medium Access Control (MAC) is lower sub-layer in the Data Link Layer
MAC is 24 bit Organizationally Unique Identifer (OUI) and 24-bit Vendor Assigned

IEEE 802.3 Ethernet Header and Trailer
Preamble                     7 bytes  Synchronization
Start Frame Delimiter (SFD)  1 byte   Next byte begins Destination MAC
Destination MAC Address      6 bytes  Identifies intended recipient of FRAME
Source MAC Address           6 bytes  Identifies sender of FRAME
Type                         2 bytes  Identifies protocol in Data field
Data and Pad                 46-1500  Higher layer data and pad bytes
Frame Check Sequence (FCS)   4 bytes  Provides for transmission error detection

MAC Broadcast Address is FFFF.FFFF.FFFF
Multicast Addresses are used for devices to voluntarily copy and forward frames
Type 0800 is IPv4
Type 86DD is IPv6
Ethernet does not attempt to recover lost frames

LAN hubs are Layer 1 devices that repeat electrical signals on all other ports.
LAN hubs lead to collisions and retransmissions using CSMA/CD (carrier sense multiple access with collision detection)
This algorithm is based on the half-duplex principle and restriction.
Devices conneted to the LAN hub may not receive while transmitting.
Full-duplex operation is possible using a Layer 2 LAN Switch which can queue one frame while sending another.
```
