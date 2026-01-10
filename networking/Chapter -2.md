# 🔥 DAY 2 – NETWORKING (DETAILED & INTENSIVE)

This document is part of a **15-Day Intensive Networking Crash Course**.  
Day 2 focuses on **addressing, segmentation, identification, and routing fundamentals**, which form the **core backbone of real-world networks**.

---

## 📘 Chapter 6: IP Addressing (IPv4)

### What is an IP Address?

An **IP (Internet Protocol) address** is a **logical address** assigned to every device in a network so that devices can **identify and communicate with each other**.

Think of it like this:

📮 **House Address → IP Address**  
🏠 **House → Computer / Device**

Without an IP address, a device cannot send or receive data on a network.

---

### IPv4 Structure

IPv4 uses:
- **32 bits**
- Divided into **4 octets**
- Written in **dotted decimal notation**

Example:

192.168.1.10


Each octet ranges from **0 to 255** because:
- 8 bits = 2⁸ = 256 values (0–255)

📌 **Real-life example:**  
Your phone connected to Wi-Fi gets an IP like `192.168.1.5`, allowing the router to identify it uniquely.

---

### IP Address Classes (With Logic)

| Class | Range (First Octet) | Network Size | Usage |
|------|-------------------|--------------|-------|
| A | 1 – 126 | Very Large | ISPs, large enterprises |
| B | 128 – 191 | Medium | Universities, organizations |
| C | 192 – 223 | Small | Home, small offices |
| D | 224 – 239 | — | Multicast |
| E | 240 – 255 | — | Research |

📌 **Easy Memory Trick**

> **A → Big**  
> **B → Medium**  
> **C → Small**  

Alphabet order = Network size order

📌 **Examples**
- `192.168.1.1` → Class C → Home network  
- `10.0.0.1` → Class A → Large corporate network  

---

## 📘 Chapter 7: Subnetting (Core Concept)

### What is Subnetting?

**Subnetting** is the process of **dividing one large network into multiple smaller networks (subnets)**.

### Why Subnetting is Required?

Subnetting is not optional in modern networks. It is required to:

- Reduce **network congestion**
- Improve **security**
- Organize networks logically
- Use IP addresses efficiently

📌 **Real-life Example**

A company has one network:
- HR Department
- Finance Department
- IT Department

Instead of one big network, subnetting creates:
- One subnet per department  
This prevents unnecessary traffic and improves security.

---

### Subnet Mask (Most Important Concept)

A **subnet mask** identifies:
- Which part of an IP is the **network**
- Which part is the **host**

Example:

IP Address : 192.168.1.10
Subnet Mask : 255.255.255.0


Meaning:
- Network portion → `192.168.1`
- Host portion → `10`

📌 **Golden Memory Rule**

> **255 = Fixed (Network)**  
> **0 = Changeable (Host)**  

---

## 📘 Chapter 8: MAC Address & ARP

### MAC Address

A **MAC (Media Access Control) address** is a **physical address** permanently assigned to a network interface card (NIC).

Characteristics:
- 48-bit address
- Written in hexadecimal
- Unique for every device

Example:

00:1A:2B:3C:4D:5E


📌 **Memory Tip**

> **MAC = Machine Address (Physical)**  
> **IP = Internet Address (Logical)**  

---

### ARP (Address Resolution Protocol)

ARP is used to **find the MAC address of a device when its IP address is known**.

---

### How ARP Works (Step-by-Step)

1. Device knows the **IP address** of destination
2. It broadcasts:  
   “Who has this IP?”
3. Destination replies with its **MAC address**
4. Communication begins using MAC address

📌 **Real-life Example**

Your laptop wants to send data to `192.168.1.5`  
ARP helps convert:

IP → MAC


---

## 📘 Chapter 9: VLAN & Trunking

### VLAN (Virtual Local Area Network)

A **VLAN** logically divides **one physical switch into multiple virtual networks**.

Important point:
- Devices in different VLANs **cannot communicate**
- Even if connected to the same switch

📌 **Real-life Example**

One switch in office:
- VLAN 10 → HR
- VLAN 20 → Finance

Even side-by-side computers remain isolated.

---

### Trunking

A **trunk link** carries **multiple VLANs through a single cable** between switches.

📌 **Memory Trick**

> **VLAN = Divide**  
> **Trunk = Carry**

---

## 📘 Chapter 10: Routing Basics

### What is Routing?

Routing is the process of **selecting the best path** to forward data from source to destination **across networks**.

Routers perform routing using **IP addresses**.

---

### Static Routing

- Manually configured
- Simple
- Suitable for small networks
- No automatic updates

📌 Example: Home or small office router

---

### Dynamic Routing

- Automatic
- Uses routing protocols
- Adapts to network changes
- Suitable for large networks

Common protocols:
- RIP
- OSPF
- EIGRP

📌 **Easy Memory Tip**

> **Static = Small Network**  
> **Dynamic = Big Network**

---

# 📝 DAY 2 – MANDATORY TEST

## Section A – MCQ

1. Which IP class is commonly used in home networks?  
2. ARP resolves which address?  
3. Which address is physical: IP or MAC?  
4. What is the main purpose of subnetting?  
5. VLAN is logical or physical?

---

## Section B – Short Answer

6. Explain IP address with example.  
7. Difference between IP address and MAC address.  
8. Explain VLAN with a real-life example.  
9. Why is subnetting required?  
10. Difference between static and dynamic routing.

---

## Section C – Long Answer

11. Explain all IP classes with ranges and usage.  
12. Explain subnet mask with a detailed example.  
13. Explain ARP working step-by-step.  
14. Explain VLAN and trunking with real-life and technical examples.

---

### ✅ End of Day 2 Documentation

## 👨‍💻 Author

**Balamutugan**
Cybersecurity | Ethical Hacking
