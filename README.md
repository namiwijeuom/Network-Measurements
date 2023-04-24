# Network-Measurements
This is an individual activity conducted under the module EN2150 Communication Network Engineering, Semester 4 of the Department of Electronic and Telecommunication Engineering, University of Moratuwa, Sri Lanka.

This activity has two stages:

Stage 1: Carry out the activities as listed below (including Wireshark packet capture)

1. What is a hierarchical network? Networks aggregating at different levels
- Tier 3 networks (typically your Internet Service Provider or Mobile Operator), Tier 2
networks, Tier 1 networks

a. Let's try to observe these hierarchical networks (Visualize the network of networks)
by using some tools.

b. Activate Wireshark packet capture and perform the following:

i. Access each of the following web pages and then Ping and Traceroute to the
same web pages. Copy the results to a file for later analysis. E.g. In your
browser open the web page www.ruh.ac.lk and then do ping www.ruh.ac.lk
followed by traceroute www.ruh.ac.lk (or tracert www.ruh.ac.lk).
1. www.ruh.ac.lk
2. www.uoregon.edu
3. www.keio.ac.jp
4. Japan.go.jp
5. nsf.gov
6. www.cam.ac.uk
7. www5.usp.br
8. www.unimelb.edu.au

ii. Stop the packet capture and save the captured packets to a file. You will
need this file later for packet dissection.

iii. Within Wireshark captured packets, analyze what happens during web page
loading, ping and traceroute by observing the packet details in each of the
layers.

iv. Why do you get "* * *" instead of IP addresses for some steps in traceroute?

v. Use IP address geographical locator to identify where a particular router is
located and to which ISP network it belongs to and to map out the physical
path the packet has taken to reach the destination.

c. What does the PING indicate?
• Compute the approx. geographical distance from your location to the end
point and compute the theoretical round trip time using speed of light in
fiber.
• Compare this with the measured ping time and analyze the reason for the
difference.
• Can you identify sub-components that contribute to PING time?
• Ping shows Round trip time (RTT), packets transmitted, packets lost, Jitter
(variation in RTT or latency)

2. Why is bandwidth (throughput) important?

a. Install iPerf : a tool used for bandwidth testing (https://iperf.fr/). If you are using Linux,
this tool may already be in the system.

b. Check public iPerf servers (https://iperf.fr/iperf-servers.php)

c. Perform iperf tests from the following places and observe and record readings.
i. At the university and at your home
ii. Do the tests during peak and off-peak traffic times.

3. Why is latency important?

a. Study about undesirable latency during network access : known as “Bufferbloat”
(https://www.bufferbloat.net/projects/)

b. Access https://www.waveform.com/tools/bufferbloat and observe and record
readings from the following places:

i. At the university, at your home, using your mobile (without connecting to
WiFi).

ii. Do the tests during peak and off-peak traffic times.

c. Install Flent - The Flexible Network Tester and go through the tutorial.

Stage 2: Analysis of the captured packets by writing your own program (Packet dissection)
