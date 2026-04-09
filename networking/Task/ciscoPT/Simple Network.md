# 🌐 Building a Simple Network in Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates how to build a **basic network topology** using Cisco Packet Tracer. It covers device setup, cable connections, IP configuration using DHCP, and testing connectivity between devices.

---

## 🎯 Objectives

* Understand basic network components
* Learn how to connect devices using appropriate cables
* Configure IP addressing using DHCP
* Verify communication between devices

---

## 🧰 Tools Used

* Cisco Packet Tracer

---

## 🟢 Part 1: Building the Network

### 🔹 Devices Used

* Personal Computer (PC)
* Laptop
* Cable Modem
* Wireless Router
* Internet Cloud

---

### 🔹 Device Roles

* **PC & Laptop** → End devices for communication
* **Wireless Router** → Connects devices and assigns IP addresses
* **Cable Modem** → Connects local network to ISP
* **Internet Cloud** → Simulates the internet

---

### 🔹 Renaming Devices

To maintain clarity:

* `PC0` → **PC**
* `Laptop0` → **Laptop**
* `CableModem0` → **Cable Modem**

---

### 🔹 Network Connections

| Connection                   | Cable Type              |
| ---------------------------- | ----------------------- |
| PC → Router                  | Copper Straight-Through |
| Router → Cable Modem         | Copper Straight-Through |
| Cable Modem → Internet Cloud | Coaxial Cable           |
| Laptop → Router              | Wireless                |

---

## 🟡 Part 2: Device Configuration

### 💻 Configuring the PC

1. Go to **Desktop → IP Configuration**
2. Select **DHCP**

✅ Result:

* PC receives IP automatically
* Example: `192.168.0.x`

---

### 💻 Configuring the Laptop

1. Remove Ethernet module
2. Install **WPC300N Wireless NIC**
3. Connect to WiFi:

   * SSID → `HomeNetwork`
4. Enable **DHCP**

✅ Result:

* Laptop receives IP automatically
* Example: `192.168.0.x`

---

## 🔵 Part 3: Testing Connectivity

### 🔹 Using Command Prompt

On PC and Laptop:

```bash
ping cisco.srv
```

---

### ✅ Expected Result

* Successful replies received
* Confirms network communication is working

---

### 🌐 Web Browser Test

* Open browser on Laptop
* Access: `cisco.srv`

✅ Confirms:

* End-to-end connectivity
* Internet access simulation working

---

## 🧠 Key Concepts Learned

### 1. DHCP (Dynamic Host Configuration Protocol)

* Automatically assigns IP addresses
* Reduces manual configuration

---

### 2. IP Addressing

* Each device needs a unique IP

**Example:**

* PC → `192.168.0.2`
* Laptop → `192.168.0.3`

---

### 3. Default Gateway

* Router acts as gateway
* Enables communication outside local network

---

## 🛠️ Troubleshooting

| Issue                 | Solution                   |
| --------------------- | -------------------------- |
| No IP Address         | Enable DHCP                |
| No connectivity       | Check cables               |
| Laptop not connecting | Install wireless NIC       |
| Ping fails            | Verify network connections |

---

## 🚀 Conclusion

This lab provided a strong foundation in networking basics. It demonstrated how devices communicate within a network and how to configure and troubleshoot connectivity issues.

---

## 🔍 Reflection

This hands-on experience improved my understanding of:

* Network setup and configuration
* Real-world connectivity concepts
* Basic troubleshooting techniques

It also builds a solid base for **cybersecurity and ethical hacking concepts**.

---

## 📎 Author

**Balamurugan**
Cybersecurity & Networking Enthusiast 🔐
