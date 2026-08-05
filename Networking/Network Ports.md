# Network Ports

A port is a logical communication endpoint used to identify a specific application or service on a device.

Think of it as:

IP Address = House Address

Port = Room Number

---

## Common Ports

| Port | Service | Protocol |
|------|----------|----------|
| 20/21 | FTP | TCP |
| 22 | SSH | TCP |
| 23 | Telnet | TCP |
| 25 | SMTP | TCP |
| 53 | DNS | UDP/TCP |
| 67 | DHCP Server | UDP |
| 68 | DHCP Client | UDP |
| 80 | HTTP | TCP |
| 110 | POP3 | TCP |
| 143 | IMAP | TCP |
| 443 | HTTPS | TCP |
| 3389 | RDP | TCP |

---

## Source Port vs Destination Port

Every network connection has:

- Source Port (chosen by the client)
- Destination Port (service port on the server)

Example

192.168.0.104:52341 → 142.250.xxx.xxx:443
