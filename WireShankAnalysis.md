# Network Traffic Analysis with Wireshark
*By Nosipho*

## What I Captured  
I used Wireshark to analyze different types of network traffic between my computer (`10.117.678.91`) and a remote server (`162.189.122.1`). Here's what I found:

---

## 1. QUIC Handshake (InitialHandShakes)
### What Happened  
When I visited a website using Chrome, my computer and the server established a secure connection using **QUIC** (the protocol behind HTTP/3).  

- **First 2 packets**: My computer sent encrypted "hello" messages  
- **Next 4 packets**: The server replied with its own encryption keys  
- **Final packet**: My computer confirmed the secure connection  

**Why this matters**: QUIC is faster than traditional HTTPS because it combines connection setup and encryption into one step!

---

## 2. Ping Test (ICMP-ECHO)
### What Happened  
I ran a simple `ping` test to check the server's response time:  

- My computer sent: *"Are you there?"* (ICMP Echo Request)  
- The server replied: *"I'm here!"* (ICMP Echo Reply)  
- **Response times varied** from 31ms to 181ms – normal network fluctuations  

**Fun fact**: If all packets failed, it would mean either:  
1. The server was offline, or  
2. A firewall was blocking my pings

---

## 3. Encrypted QUIC Traffic (ProtectedPayloads)
### What Happened  
After the handshake, all communication was encrypted:  

- **Small packets (86 bytes)**: Basic *"message received!"* acknowledgments  
- **Larger packets (467 bytes)**: Actual website data being transferred  
- Every packet showed **"Protected Payload"** – meaning no one could spy on my browsing  

**Key takeaway**: This is how modern browsers keep your banking/shopping sessions secure!

---

## How I Analyzed This  
1. Used Wireshark filters like `quic` and `icmp` to isolate traffic  
2. Checked packet details to understand the encryption process  
3. Compared timing between requests/replies to measure performance  

---

## Why This Matters  
Understanding these basics helps with:  
🔹 **Debugging network issues** (e.g., why a website loads slowly)  
🔹 **Security awareness** (how encryption protects data)  
🔹 **Future learning** (this is the foundation of protocols like HTTP/3)  

> *Note: All captures contain only outbound traffic from my personal device to public servers. No sensitive data is included.*
