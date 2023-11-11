# Analyzing network traffic with Wireshark


<h2>Introduction to Wireshark</h2>

Wireshark is an essential tool used in the networking industry to analyze network protocols. It can be used to capture many different types of network traffic; often mainly used to troubleshoot problems in a network such as latency issues, detecting malicious traffic, observing network traffic, and much more. Wireshark is one of the most helpful tools when it comes to networking. Since it has a GUI it is fairly simple to learn and user friendly. With colors to distinguish between different types of traffic, Wireshark is very straightforward.
<hr>

<h2>Observing ICMP echo request/reply packets with Wireshark</h2>

This demonstration will be going over how to analyze ICMP echo request and echo reply packets between two different hosts. The point of this demonstration is to help the user gain more insight into network communication.

<strong>Opening Wireshark:</strong>

When Wireshark is opened, the first thing the user is greeted with is a screen with a list of available interfaces to capture. This example will be capturing network traffic from "eth0" (ethernet interface) which is basically the network connection. 
<hr>

![etho](https://github.com/victorF29/Wireshark/assets/145622790/37149c1c-1e75-408e-92fc-6f43b474871f)
<hr>
<strong>Analyzing captured packets:</strong>

Once inside the network interface, a blank list will pop up where captured network packets can be found. This list begins to populate itself once Wireshark is able to capture any network packets that get recieved or sent out.
<hr>

![blank](https://github.com/victorF29/Wireshark/assets/145622790/ca2bf9e1-4154-4c26-a80c-2b0e53683222)
<hr>

To begin populating Wireshark with packets, the ping command will be used to capture packets sent between two hosts. For the most part the ping command is used to check whether or not a host is running. The source computer will send a request to the destination, and the destination will either reply or not reply depending on whether or not it is up. Once the list begins to populate, many different kinds of packets will start to show. Each different packet will show a different color depending on the protocol. In the screenshot below there are two different protocols shown, ARP and ICMP. ARP is used for linking a MAC address to an IP address, this is so that the two hosts can communicate with each other. The ICMP protocol is a protocol used for diagnosing things on networks; in this case using ping to see if the destination is up.
<hr>

![listofpacks](https://github.com/victorF29/Wireshark/assets/145622790/9f350bdf-b0f0-4879-8d20-1c654cfd22bc)
<hr>

At the top of Wireshark there is a search bar used to filter through packets. Typing in ICMP shows only packets that have ICMP protocol. The search feature can be used with much greater detail to be able to find more specific things. Clicking on an individual packet will bring up more information on that specific packet. The picture below shows the specific detail for the given packet clicked, this is shown at the bottom half of Wireshark. Shown at the bottom of the list are things such as host source and host destination, the byte size of the packets, what interface the packet was captured on, along with other details. Clicking on the drop down that says "Internet Control Message Protocol" shows even more detail about the packet such as the type of packet. In this case type 8 which means this is an echo ping request. As well as the time the packet was captured, and the integrity of the packet (checksum).
<hr>

![icmp](https://github.com/victorF29/Wireshark/assets/145622790/2960a4b1-35f6-4527-b2ee-33e62fe871a3)
<hr>

The screenshot provided shows an example of how it looks like when a host does not send a reply back. In this case the destination host does not exist.
<hr>

![down](https://github.com/victorF29/Wireshark/assets/145622790/4d8c37d1-71b4-46a7-a786-2cda77174563)
<hr>

<h2>Concepts of this demonstration</h2>

This demonstration showed off the basics in how to use Wireshark, how to capture and analyze ICMP echo request/reply packets, as well as reading through some of the packets data. As well as showing how Wireshark can be used to gain more insight into a networks communication, how to capture packets on a network, and how to interpret packet data. Wireshark has many use cases from being able to diagnose problems in a network, to monitoring whats going on in a network, and overall having more insight as to whats going on in a network. 
