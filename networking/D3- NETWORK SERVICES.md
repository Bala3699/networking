---

# 📘 DAY 3 — CORE NETWORK SERVICES

---

## 3.0 Overview of Core Network Services

Core Network Services form the **foundation of computer networking**.
They define **how devices are identified**, **how they locate each other**, and **how data is delivered across networks**.

Every modern network—home, office, data center, or the internet—relies on these services to function correctly.

This chapter covers:

* IP Addressing
* MAC Addressing
* ARP (Address Resolution Protocol)
* Subnet Mask
* VLAN
* Routing (Basics)

---

## 3.1 IP Addressing

### Concept

An **IP Address (Internet Protocol Address)** is a **logical identifier** assigned to a device in a network.
It allows devices to **identify and communicate** with each other.

Unlike hardware addresses, IP addresses **can change** depending on the network.

---

### Structure of IPv4 Address

An IPv4 address consists of:

* **32 bits**
* Divided into **4 octets**
* Each octet ranges from **0–255**

📌 Example:

```
192.168.12.1
```

Each part is separated by a dot and together forms a **unique logical address**.

---

### Purpose of IP Addressing

IP addressing enables:

* Device identification
* Location identification
* Routing of data between networks

📌 Real-Life Analogy
IP address is like a **home address**:

* City → Network
* House number → Device

---

### IP Address Classes

IP addresses are divided into classes based on network size:

| Class | Range   | Usage               |
| ----- | ------- | ------------------- |
| A     | 1–126   | Very large networks |
| B     | 128–191 | Medium networks     |
| C     | 192–223 | Small networks      |
| D     | 224–239 | Multicast           |
| E     | 240–255 | Research            |

📌 **Memory Tip**
Class **C = Common LANs** (homes, offices)

---

## 3.2 MAC Address

### Concept

A **MAC Address (Media Access Control Address)** is a **physical address** permanently assigned to a network interface card (NIC) by the manufacturer.

It is:

* 48-bit long
* Written in hexadecimal format
* Unique worldwide

📌 Example:

```
00:1A:2B:3C:4D:5E
```

---

### Role of MAC Address

MAC addresses are used for **local network communication** (LAN).
Ethernet devices rely on MAC addresses to **deliver frames** to the correct device.

📌 Key Difference

* IP Address → Logical, changeable
* MAC Address → Physical, permanent

📌 Memory Tip
**MAC = Machine Address**
**IP = Internet Address**

---

## 3.3 ARP (Address Resolution Protocol)

### Concept

ARP is a protocol used to **map an IP address to a MAC address** within a local network.

---

### Why ARP Is Required

Communication inside a LAN happens using **MAC addresses**, but users and applications work with **IP addresses**.

ARP acts as the **translator** between IP and MAC.

---

### Working of ARP (Step-by-Step Flow)

1. A device knows the **IP address** of the destination
2. It does not know the **MAC address**
3. ARP sends a **broadcast request**:

   > “Who has this IP address?”
4. The correct device responds with its MAC address
5. Communication begins using MAC addresses

📌 Example
Device wants to contact `192.168.1.5`
ARP finds → `AA:BB:CC:DD:EE:FF`

📌 Memory Tip
**ARP = IP → MAC**

---

## 3.4 Subnet Mask

### Concept

A **Subnet Mask** defines **which part of an IP address is the network portion and which part is the host portion**.

It works **together with the IP address**.

---

### Common Subnet Mask

```
255.255.255.0
```

---

### How Subnet Mask Works

Binary representation:

```
255 = 11111111
0   = 00000000
```

Subnet mask:

```
11111111.11111111.11111111.00000000
```

* `1` → Network part
* `0` → Host part

---

### Practical Example

```
IP Address:   192.168.1.10
Subnet Mask: 255.255.255.0
```

* Network portion → `192.168.1`
* Host portion → `10`

All devices with:

```
192.168.1.X
```

belong to the **same network**.

📌 Memory Tip
**255 = Fixed (Network)**
**0 = Changeable (Host)**

---

## 3.5 VLAN (Virtual LAN)

### Concept

A VLAN logically divides **one physical switch** into **multiple virtual networks**.

Devices in different VLANs:

* Cannot communicate directly
* Even if connected to the same switch

---

### Purpose of VLAN

VLANs are used to:

* Reduce network traffic
* Improve security
* Organize departments logically

---

### Example

One physical switch:

* VLAN 10 → HR Department
* VLAN 20 → Finance
* VLAN 30 → IT

Even though all devices use the same switch, they behave as **separate networks**.

📌 Memory Tip
**VLAN = Logical separation**

---

## 3.6 Trunking

### Concept

A **Trunk link** carries traffic from **multiple VLANs over a single physical cable**.

---

### Why Trunking Is Needed

When VLANs exist on multiple switches, trunking allows:

* VLAN information to travel between switches
* Efficient use of cables

📌 Example
One trunk cable carries:

* VLAN 10
* VLAN 20
* VLAN 30

📌 Memory Tip
**VLAN = Divide**
**Trunk = Carry**

---

## 3.7 Routing (Introduction)

### Concept

Routing is the process of **forwarding data between different networks** using a router.

Routers operate at the **Network Layer (Layer 3)** and use **IP addresses**.

---

### Types of Routing

**Static Routing**

* Manually configured
* Suitable for small networks

**Dynamic Routing**

* Automatically updates routes
* Uses protocols like RIP, OSPF

📌 Memory Tip

**Static = Small**

**Dynamic = Big**

---


