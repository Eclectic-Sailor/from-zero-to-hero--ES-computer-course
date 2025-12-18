# L16: Networking Deeper (EO5)
**Objectives:** TCP handshake details, DNS, Wireshark basics, sockets concept.

## Resources
- Watch: NetworkChuck Wireshark basics (~20m): https://www.youtube.com/watch?v=3F1d3QWsyk0
- Read: TCP 3-way handshake primer: https://www.geeksforgeeks.org/tcp-3-way-handshake-process/
- Congestion control overview: https://cs.nyu.edu/courses/fall13/CSCI-GA.2262-001/notes/lecture6.pdf

## Tasks
- Capture packets: run `ping example.com` and capture with Wireshark or tcpdump; identify SYN, SYN-ACK, ACK.
- Capture an HTTP request; locate DNS query/response for the host.
- Sketch a high-level socket flow: server `bind/listen/accept`, client `connect/send/recv`.

## Example to Analyze
- Look at a TCP packet: what are source/dest ports, sequence/ack numbers?

## Knowledge Check
- Why do we need a handshake?
- What problem does congestion control solve?
- How does DNS caching help performance?

## Exit Criteria
- You can label handshake packets and a DNS query/answer in a capture.
- You can describe the lifecycle of a TCP connection and where DNS fits.
