# 🚀 Networking Crash Course – Day 1 (Intensive)

This is **Day 1** of a **15-day intensive networking study plan**.  
We cover **5 chapters in detail**: Introduction to Networking, OSI Model, TCP/IP Model, Network Devices, Network Topologies.  

This file is suitable for **GitHub storage** and revision.

---

## 📘 Chapter 1: Introduction to Networking

### What is a Computer Network?
A **computer network** is a collection of **interconnected devices** (computers, servers, printers, routers) that communicate using **rules called protocols** to exchange data.  

### Why Networking is Important
- **Resource Sharing:** Printers, storage, internet.  
- **Communication:** Email, chat, video calls.  
- **Centralized Management:** Easier to maintain systems.  
- **Cost Reduction:** Shared resources reduce expenses.  
- **Internet Access:** Connect multiple devices to the global network.

### Network Types

| Type | Area | Speed | Example |
|------|------|-------|---------|
| LAN (Local Area Network) | Small area, like office or lab | High | College lab |
| WAN (Wide Area Network) | Large area, cities or countries | Low | Internet connecting multiple cities |
| MAN (Metropolitan Area Network) | City-wide | Medium | City Wi-Fi network |
| PAN (Personal Area Network) | Very small area (personal devices) | Medium | Bluetooth, USB tethering |

---

## 📘 Chapter 2: OSI Model (Open Systems Interconnection)

### Why OSI Model Exists
- Standardizes communication across networks.  
- Helps in **troubleshooting network problems**.  
- Designs **interoperable systems**.

### OSI Layers

| Layer | Function | Example |
|-------|---------|---------|
| 7. Application | Interface between user & network | Web browser (HTTP/HTTPS), Email client (SMTP) |
| 6. Presentation | Encryption, decryption, compression | HTTPS, JPEG, ASCII conversion |
| 5. Session | Manage sessions | Zoom call connection, FTP session |
| 4. Transport | End-to-end delivery, error checking | TCP (reliable), UDP (fast) |
| 3. Network | Routing, IP addresses | Routers forwarding packets |
| 2. Data Link | MAC addresses, error detection | Switches forwarding frames |
| 1. Physical | Bits, cables, wireless signals | NIC, hubs, fiber optic cables |

**Mnemonic:** *All People Seem To Need Data Processing*

**Text Diagram:**
```
+---------------------+
| Application Layer | 7
+---------------------+
| Presentation Layer | 6
+---------------------+
| Session Layer | 5
+---------------------+
| Transport Layer | 4
+---------------------+
| Network Layer | 3
+---------------------+
| Data Link Layer | 2
+---------------------+
| Physical Layer | 1
+---------------------+
```


**Real Example:** Sending an email:  
- Application → Gmail  
- Presentation → Encrypt  
- Session → Keep connection  
- Transport → TCP ensures delivery  
- Network → Routing via IP  
- Data Link → MAC forwarding via switch  
- Physical → Transmit bits via cable

---

## 📘 Chapter 3: TCP/IP Model

### Why TCP/IP is Important
- It is the **foundation of the Internet**.  
- It is **practical and widely used**, unlike OSI (theoretical).  

### TCP/IP Layers

| Layer | Function | Protocols/Examples |
|-------|---------|------------------|
| Application | Interface for apps | HTTP, FTP, SMTP, DNS |
| Transport | End-to-end delivery | TCP (reliable), UDP (fast) |
| Internet | Routing, addressing | IP, ICMP |
| Network Access | Physical transmission | Ethernet, Wi-Fi |

**Comparison with OSI:**
- OSI: 7 layers, theoretical, good for understanding.  
- TCP/IP: 4 layers, practical, used in Internet.

---

## 📘 Chapter 4: Network Devices

| Device | Layer | Function | Example |
|--------|-------|---------|---------|
| Router | 3 | Connects networks, IP routing | Home router connecting LAN → Internet |
| Switch | 2 | Connects devices in LAN using MAC | Office LAN |
| Hub | 1 | Broadcasts data to all ports | Obsolete |
| Access Point | 2/1 | Wireless connectivity | Wi-Fi hotspot |
| Firewall | 3/4 | Security, block unauthorized access | Network security appliance |
| Repeater | 1 | Boosts signal | Extending Wi-Fi range |
| Bridge | 2 | Connects LAN segments | Office network expansion |

---

## 📘 Chapter 5: Network Topologies

| Topology | Description | Advantages | Disadvantages | Example |
|----------|------------|------------|---------------|---------|
| Star | Central switch/hub | Easy to install, troubleshoot | Central device failure stops network | Office LAN |
| Bus | Single backbone cable | Cheap, easy | Collisions, limited devices | Old Ethernet networks |
| Ring | Circular path | Orderly access using token | One failure can disrupt | Token Ring LAN |
| Mesh | Every node connected | High redundancy, fault tolerant | Expensive, complex cabling | Data centers, backbone network |
| Hybrid | Combination | Flexible | Complex | Large enterprise network |

---

## 📝 Day 1 Test

### Section A – MCQ

1. Which layer handles encryption? → **Presentation Layer**  
2. Router works at which layer? → **Network Layer**  
3. Which topology uses backbone cable? → **Bus Topology**  
4. TCP is used at which layer? → **Transport Layer**  
5. Switch uses which address? → **MAC Address**

---

### Section B – Short Answer

**6. Define networking:**  
Interconnected devices exchanging data using protocols for communication and resource sharing.  

**7. OSI layers in order:**  
Application → Presentation → Session → Transport → Network → Data Link → Physical  

**8. TCP vs UDP:**

| Feature | TCP | UDP |
|---------|-----|-----|
| Connection | Oriented | Connectionless |
| Reliability | Reliable | Unreliable |
| Speed | Slower | Faster |
| Example | File transfer | Video streaming |

**9. Hub vs Switch:**

| Feature | Hub | Switch |
|---------|-----|--------|
| Layer | 1 | 2 |
| Address | None | MAC |
| Speed | Slow | Fast |
| Security | Low | High |

**10. What is MAN?**  
Metropolitan Area Network covering a city, faster than WAN, larger than LAN. Example: City-wide Wi-Fi.

---

### Section C – Long Answer

**11. Explain OSI Model:**  
- 7 layers for standardization, troubleshooting, interoperability.  
- See diagram above.  
- Real example: Email, video call, file transfer.

**12. Compare OSI & TCP/IP:**

| Feature | OSI | TCP/IP |
|---------|-----|--------|
| Layers | 7 | 4 |
| Type | Theoretical | Practical |
| Focus | Understanding, design | Internet implementation |
| Protocols | HTTP, FTP, TCP, IP etc. | HTTP, TCP, IP, UDP |

**13. Router vs Switch:**  
- Router: Layer 3, IP-based routing, LAN → WAN  
- Switch: Layer 2, MAC-based forwarding, LAN devices  

**14. Star vs Mesh Topology:**  
- Star: Central device, easy maintenance, but single point of failure  
- Mesh: Every node connected, very reliable, expensive and complex  

---

### ✅ References / Notes

- Real-time examples used for **easy memory retention**  
- Diagrams included for **GitHub Markdown readability**  
- Test answers included for **self-evaluation**  

---

**End of Day 1 Documentation**

---

## 👨‍💻 Author

**Balamutugan**
Cybersecurity | Ethical Hacking 
