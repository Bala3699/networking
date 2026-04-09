# 🏠 Smart Home IoT Network Setup using Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the setup and configuration of a **Smart Home IoT Network** using Cisco Packet Tracer. It includes exploring an existing network, adding wireless and wired IoT devices, and ensuring proper communication between devices through a Home Gateway.

---

## 🎯 Objectives

* Explore an existing smart home network
* Add and configure wireless IoT devices
* Add and configure wired IoT devices
* Establish communication between IoT components

---

## 🧰 Tools Used

* Cisco Packet Tracer

---

## 🟢 Part 1: Exploring the Existing Network

### 🔍 Steps Performed

* Navigated to **End Devices → Home** to view available IoT devices
* Observed device details like IP address by hovering over devices
* Tested devices using **Alt + Click**
* Accessed **Home Gateway configuration**:

  * Retrieved IP Address
  * Noted SSID (WiFi Name)
  * Recorded WPA2 Passphrase
* Used **Tablet → Web Browser** to:

  * Login to Home Gateway (`admin/admin`)
  * Monitor and control IoT devices

---

## 📶 Part 2: Adding a Wireless IoT Device (Wind Detector)

### ⚙️ Configuration Steps

1. Added **Wind Detector** from End Devices
2. Set:

   * Display Name → `Wind Detector`
   * IoT Server → Home Gateway
3. Configured Wireless:

   * Authentication → WPA2-PSK
   * Entered correct passphrase
4. Verified connection via Tablet

### ✅ Result

* Wind Detector successfully connected and visible in IoT device list

---

## 🔌 Part 3: Adding a Wired IoT Device (Smart Sprinkler)

### ⚙️ Configuration Steps

1. Added **Lawn Sprinkler**
2. Enabled network adapter:

   * Advanced → I/O Config → `PT-IOT-NM-1CFE`
3. Connected using:

   * **Copper Straight-Through Cable**
4. Configured:

   * Display Name → `Smart Sprinkler`
   * IoT Server → Home Gateway
   * IP Configuration → DHCP

### ✅ Result

* Smart Sprinkler received IP address and appeared in network

---

## 🔗 Part 4: Adding Water Meter and Device Integration

### ⚙️ Configuration Steps

1. Added **Water Level Monitor**
2. Set:

   * Display Name → `Water Meter`
   * IoT Server → Home Gateway
3. Configured Wireless:

   * Connected to Home Gateway SSID
   * Entered passphrase
4. Enabled I/O:

   * Digital Slots → 1
   * Usage → Component
5. Connected to Smart Sprinkler using:

   * **IoT Custom Cable (D0 to D0)**

### ✅ Result

* Water Meter successfully connected and integrated with Smart Sprinkler

---

## 🧪 Verification

* Used **Tablet / Smartphone browser**
* Logged into Home Gateway
* Verified all devices:

  * ✔ Wind Detector
  * ✔ Smart Sprinkler
  * ✔ Water Meter

---

## ⚠️ Challenges Faced

* IoT Server not updating correctly
* Device not getting IP address initially
* Incorrect cable type used
* Packet Tracer scoring mismatch despite correct configuration

---

## 🛠️ Solutions

* Reconfigured IoT Server (set to None → Home Gateway)
* Enabled DHCP on Home Gateway
* Used correct cable types:

  * Wireless → WPA2-PSK
  * Wired → Copper Straight-Through
  * IoT → Custom Cable
* Ensured correct naming conventions (case-sensitive)
* Restarted Packet Tracer to fix scoring issues

---

## 🧠 Key Learnings

* Importance of correct configuration sequence
* Understanding IoT device communication
* Difference between wired and wireless IoT setup
* Role of Home Gateway in IoT networks
* Troubleshooting common network issues

---

## 🚀 Conclusion

The smart home network was successfully configured with both wired and wireless IoT devices. All devices were able to communicate via the Home Gateway, demonstrating a functional IoT ecosystem within Cisco Packet Tracer.

---

## 📎 Author

**Balamurugan**
Cybersecurity & Networking Enthusiast 🔐
