# Analyzing network traffic with Wireshark


<h2>Introduction to Wireshark</h2>

Wireshark is an essential tool used in the networking industr to analyze network protocols. It can be used to capture many different types of network traffic; often mainly used to troubleshoot problems in a network such as latency issues, detecting malicious traffic, observing network traffic, and much more. Wireshark is one of the most helpful tools when it comes to networking. Since it has a GUI it is fairly simple to learn and user friendly. With colors to distinguish between different types of traffic, Wireshark is very straightforward.
<hr>

<h2>Observing ICMP echo request/reply packets with Wireshark</h2>

This demonstration will be going over how to analyze ICMP echo request and echo reply packets between two different hosts. The point of this demonstration is to show off how Wireshark works and show the basics of how to capture and analyze traffic between two seperate hosts.

<strong>Opening Wireshark:</strong>

When Wireshark is opened, the first thing the user is greeted with is a screen with a list of available interfaces to capture. This example will be capturing network traffic from "eth0" (ethernet interface) which is basically the network connection. 
<hr>

![etho](https://github.com/victorF29/Wireshark/assets/145622790/37149c1c-1e75-408e-92fc-6f43b474871f)
<hr>
<strong>Analyzing captured packets:</strong>

Once inside the network interface, a blank list will pop up where captured network packets can be found. This list begins to populate itself once Wireshark is able to capture any network packets that get recieved or sent out.
<hr>

![blank](https://github.com/victorF29/Wireshark/assets/145622790/ca2bf9e1-4154-4c26-a80c-2b0e53683222)
