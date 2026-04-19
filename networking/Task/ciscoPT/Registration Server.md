# 📡 Packet Tracer Lab: Connect IoT Devices to a Registration Server

## 🧑‍💻 Author

**Balamurugan (Cybersecurity & Networking Enthusiast)**

---

## 📌 Overview

This lab demonstrates how to:

* Register IoT devices to a remote IoT server
* Monitor IoT devices through a web interface
* Configure **cellular tethering** between a smartphone and a laptop
* Verify network connectivity using real-time simulation

---

## 🎯 Objectives

### 🔹 Part 1: Register IoT Devices to the Registration Server

* Access IoT devices via Home Gateway
* Register devices to a remote server (`home.com`)
* Verify successful device registration

### 🔹 Part 2: Connect a Smartphone to a Laptop Using Tethering

* Enable Bluetooth communication
* Pair smartphone with laptop
* Use cellular data to provide internet access

---

## 🧠 Background

In modern IoT environments, devices are often managed through centralized servers rather than local gateways. This allows:

* Remote monitoring
* Centralized control
* Scalable architecture

Additionally, **tethering** enables devices without direct internet access to connect via mobile networks.

---

# 🏠 Part 1: Register IoT Devices to Remote Server

## 🔸 Step 1: Access IoT Devices from Home Gateway

1. Open the **Tablet**
2. Navigate to:

   ```
   Desktop → IoT Monitor
   ```
3. Click **Login** (default credentials)
4. Observe currently registered IoT devices

---

## 🔸 Step 2: Access Remote IoT Server

1. Open **Web Browser** (Tablet)
2. Enter:

   ```
   http://home.com
   ```
3. Login credentials:

   ```
   Username: home  
   Password: home
   ```
4. Notice:

   * No devices are listed (yet)

---

## 🔸 Step 3: Register IoT Devices

### ⚙️ Configure Each Device (Fan, Lamp, Door)

For each device:

1. Open device (e.g., **Fan**)
2. Go to:

   ```
   Config → IoT Server
   ```
3. Change:

   ```
   Server Type: Home Gateway → Remote Server
   ```
4. Enter:

   ```
   Server Address: home.com  
   Username: home  
   Password: home
   ```
5. Click **Connect**

✔ Repeat for:

* Fan
* Lamp
* Door

---

## 🔸 Step 4: Verify Registration

1. Return to:

   ```
   Browser → home.com
   ```
2. Login again
3. Check **IoT Devices List**

✅ Expected Output:

* Fan → Online
* Lamp → Online
* Door → Online

📌 If devices show **Offline**:

* Reopen device config
* Click **Refresh / Reconnect**

---

# 📱 Part 2: Smartphone Tethering (Bluetooth)

## 🔸 Step 1: Enable Bluetooth on Laptop

1. Open **Laptop**
2. Go to:

   ```
   Config → Bluetooth
   ```
3. Set:

   ```
   Port Status → ON
   ```

---

## 🔸 Step 2: Enable Bluetooth on Smartphone

1. Open **Smartphone**
2. Ensure:

   * Connected to **Cellular Network (3G/4G)**
3. Click:

   ```
   DHCP Refresh
   ```
4. Enable:

   ```
   Bluetooth → ON
   ```

---

## 🔸 Step 3: Pair Smartphone with Laptop

### 📲 On Smartphone:

1. Go to:

   ```
   Config → Bluetooth
   ```
2. Click **Discover**
3. Select **Laptop**
4. Click **Pair**

✔ Accept pairing request

---

### 💻 On Laptop:

1. Open:

   ```
   Config → Bluetooth
   ```
2. Select **Smartphone**
3. Click **Tether**

---

## 🔸 Step 4: Verify Connectivity

### 🖥 Test via Command Prompt

```bash
ping home.com
```

✅ Expected Result:

* Successful replies
* Internet connectivity established

---

### 🌐 Browser Test

1. Open browser on Laptop
2. Visit:

   ```
   http://home.com
   ```
3. Login and view IoT devices

---

# 📊 Key Concepts Learned

* IoT Device Registration (Local vs Remote Server)
* Cloud-based IoT Management
* Bluetooth Pairing & Tethering
* Cellular Network Integration
* Network Connectivity Testing (Ping)

---

# ⚠️ Common Issues & Fixes

| Issue                | Solution               |
| -------------------- | ---------------------- |
| Devices show Offline | Reconnect to server    |
| No IP on smartphone  | Use DHCP Refresh       |
| Pairing fails        | Restart Bluetooth      |
| Ping fails           | Check tethering status |

---

# 🚀 Real-World Applications

* Smart Home Automation Systems
* Remote IoT Monitoring Platforms
* Mobile Network Failover Systems
* Emergency Internet Access via Tethering

---

# 📌 Conclusion

This lab provides hands-on experience in:

* Managing IoT devices remotely
* Integrating mobile networks into traditional networking
* Understanding real-world IoT infrastructure

It bridges the gap between **network simulation and practical IoT deployment**.

---

# 🔗 Future Improvements

* Add **MQTT protocol integration**
* Implement **IoT security (authentication, encryption)**
* Simulate **IoT attacks and monitoring**
* Integrate with your **CyberSentinel project** 🔐

