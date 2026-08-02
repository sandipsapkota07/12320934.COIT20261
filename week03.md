# COIT20261 Portfolio – Week 03

**Student Name:** Sandip Sapkota  
**Student ID:** 12320934  
**Week:** 03

---

# Objective

The objective of this tutorial was to learn how to use Netcat (nc) for simple client-server communication and to capture network traffic using GNS3.

---

# Task 1 – Netcat Communication

## Activities Completed

I used the existing `Setting-IP-12320934` project containing four Linux hosts connected through an Ethernet switch.

The following steps were completed:

- Started the Netcat server on Host A.
- Used TCP port **12345**.
- Connected Host C to the server using the server's IP address.
- Sent my name from the client to the server.
- Sent my student ID from the server to the client.

---

## Commands Used

### Server

```bash
nc -l -p 12345
```

### Client

```bash
nc 10.1.0.1 12345
```

---

## Result

The client successfully connected to the server and messages were exchanged in both directions.

---

## Evidence

### Netcat Server

![Netcat Server](images/week03-netcat-server.png)

### Netcat Client

![Netcat Client](images/week03-netcat-client.png)

---

# Task 2 – Packet Capture

## Activities Completed

Packet capture was started on the link between Host A and the Ethernet switch.

While the capture was running:

- Sent three ICMP Echo Requests using ping.
- Established a Netcat connection.
- Sent a text message through Netcat.
- Stopped the packet capture.
- Used FileZilla to transfer the capture file from the GNS3 server to the Windows host computer.

---

## Commands Used

### Ping

```bash
ping -c 3 10.1.0.2
```

### Netcat

```bash
nc 10.1.0.1 12345
```

---

## Capture File

```
12320934-ping-netcat.pcap
```

---

## Evidence

### Ping Output

![Ping](images/week03-ping.png)

### Packet Capture Transfer

![FileZilla](images/week03-filezilla.png)

---

# Testing Results

| Test | Result |
|------|--------|
| Netcat server started successfully | Pass |
| Netcat client connected successfully | Pass |
| Name sent successfully | Pass |
| Student ID received successfully | Pass |
| Ping packets transmitted | Pass |
| Packet capture completed | Pass |
| PCAP file transferred successfully | Pass |

---

# Reflection

This tutorial helped me understand the difference between application-layer communication and network-layer communication. I learned how Netcat can be used to establish a simple TCP connection between two hosts and exchange text messages.

I also learned how to capture network traffic in GNS3 and transfer the capture file to my Windows computer using FileZilla. This practical activity demonstrated how communication between hosts can be recorded for later analysis using Wireshark.

---

# Learning Outcomes

After completing this tutorial, I can:

- Use Netcat as a simple TCP server and client.
- Exchange messages between Linux hosts.
- Test connectivity using the ping command.
- Capture packets in GNS3.
- Transfer packet capture files from the GNS3 server to my computer using FileZilla.
