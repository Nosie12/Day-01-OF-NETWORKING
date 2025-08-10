# Networking Basics

---

## 🚀 Welcome to the Course

- Cisco’s CCNA Certification is a great way to learn networking.
- The course includes videos, quizzes, online simulations, and lab guides.
- Hands-on practice with Cisco CLI and simulators (routers, switches) is essential.
- Networking knowledge focuses on practical skills, not just theory.

---

## 🔑 What is a Network?

- A network is simply two or more devices connected to share information.
- Examples: Two PCs connected by an Ethernet cable or a home network with wireless devices.
- Networks let devices like computers, phones, and printers communicate and share resources.

---

## 📡 Network Interface Card (NIC)

- A NIC (also called network adapter) connects your device to the network.
- Can be wired (Ethernet card) or wireless (Wi-Fi adapter).
- Enables devices to send/receive data over the network.

---

## 🛑 What is a Network Protocol?

- A set of rules that govern how devices communicate on a network.
- Like human languages: devices must “speak” the same protocol to understand each other.
- Example: IP (Internet Protocol) is the language for addressing and routing data.
- Network communication is governed by rules similar to traffic lights: green means go, red means stop.
- Different protocols exist for different tasks; we’ll cover many in this course.
- The **OSI Model** explains network communication in 7 layers (to be covered later).

---

## 🏠 Home Network Overview

- Typical home network:
  - Router connected to the internet via DSL, cable, or broadband.
  - Devices connect to the router via Ethernet or Wi-Fi.
  - Switches may be used to expand wired connections.
- Routers forward data between devices or to the internet by making routing decisions.
- Similar to choosing driving routes based on distance or traffic.
- Tools like **Ping** and **Traceroute** test network connectivity and routes.

---

## 🌐 What is an IP Address?

- IP Address = unique numeric identifier for each device on a network.
- Acts like a home address, so data can find the right device.
- IPs can be:
  - **Static** (manually set)
  - **Dynamic** (automatically assigned via DHCP)
- Routers and servers allocate IPs dynamically to devices joining the network.

---

## 🔢 IP Versions and Address Classes

- IPv4 (most common) and IPv6 (newer, larger address space).
- IP addresses have classes (A, B, C, D, E) defining network size and purpose.
- Special IPs include:
  - Loopback addresses (for self-testing)
  - Broadcast addresses (to send data to all devices in a network)
  - Private IP ranges (used inside local networks)
- Network masks (subnets) help divide IP addresses into networks and hosts.

---

## 🌐 Domain Name System (DNS)

- DNS converts human-friendly domain names (e.g., `google.com`) into IP addresses.
- Like a phonebook for the internet, so you don’t have to remember numeric IPs.
- Tools:
  - `ping domain.com`: tests connectivity and shows the IP address.
  - `traceroute domain.com`: shows the path data takes through routers to reach a destination.
- Your network usually assigns DNS servers automatically, but you can configure custom ones (e.g., Google DNS).

---

## 📡 Wired vs Wireless Connections

- Wired uses Ethernet or fiber cables.
- Wireless uses radio waves (Wi-Fi).
- Wireless NICs allow devices to send/receive data over the air like a radio.
- Devices can both transmit and receive wirelessly, unlike traditional radio receivers.

---

## 🧰 Useful Tools and Concepts

- **Ping**: Check if a device or website is reachable.
- **Traceroute**: View the path data takes through routers to reach a destination.
- **Router**: Directs traffic between devices and networks.
- **Switch**: Connects multiple devices on the same network physically.

---

## 📚 Summary

- Networking connects devices to share data and resources.
- Protocols set the rules for communication.
- IP addresses uniquely identify devices on a network.
- DNS translates easy-to-remember domain names into IP addresses.
- Routers and switches move data efficiently.
- Understanding physical (cables, wireless) and logical (protocols) connections is key.
- Hands-on practice with simulators and tools is crucial for learning.

---
