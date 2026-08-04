# Networking Learning Journey

# Transmission Control Protocol (TCP)

Transmission Control Protocol (TCP) is a **connection-oriented** protocol that establishes a connection between the sender and the receiver before transmitting data.

TCP ensures that data is delivered **accurately, reliably, and in the correct order**. If any packet is lost during transmission, TCP detects the loss and retransmits the missing packet.

TCP uses a **3-way handshake** to establish a connection:

1. SYN – The client requests a connection.
2. SYN-ACK – The server acknowledges the request and responds.
3. ACK – The client acknowledges the server's response, and the connection is established.

## Features
- Connection-oriented
- Reliable data delivery
- Error checking
- Packet retransmission
- Ordered data delivery

## Common Uses
- HTTP/HTTPS
- FTP
- SSH
- Email (SMTP, IMAP, POP3)


- # User Datagram Protocol (UDP)

User Datagram Protocol (UDP) is a **connectionless** protocol that sends data without establishing a connection between the sender and the receiver.

Unlike TCP, UDP does **not** guarantee that data will be delivered, received in the correct order, or retransmitted if packets are lost. Because it skips these reliability checks, UDP is **faster** and has **lower latency** than TCP.

UDP is mainly used in applications where speed is more important than reliability.

## Features
- Connectionless
- Faster than TCP
- Low latency
- No error recovery
- No packet retransmission
- No guaranteed delivery
- No ordered data delivery

## Common Uses
- DNS
- VoIP (Voice over IP)
- Online Gaming
- Video Streaming
- Live Broadcasting
