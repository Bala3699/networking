
# 🖧 Packet Tracer – Realistic Structured Cabling in the Physical Workspace

## 📌 Overview
This project demonstrates how to create a realistic structured cabling environment using Cisco Packet Tracer. The lab simulates how office devices are connected through wall mounts, patch panels, and switches inside a wiring closet.

The project includes:

- Installing a Patch Panel
- Adding Wall Mounts
- Connecting Switch Ports to Patch Panel
- Connecting Wall Mounts to Patch Panel
- Connecting PCs and Printer to the Network
- DHCP IP Address Assignment
- Testing Connectivity using a Web Browser

---

# 🎯 Objectives

- Understand structured cabling concepts
- Learn how patch panels work
- Learn wall mount and punchdown connections
- Simulate enterprise office network cabling
- Configure realistic office infrastructure

---

# 🏢 Network Topology

```text
Office Devices
      ↓
Wall Mounts
      ↓
Patch Panel
      ↓
Switch
      ↓
Server
````

---

# 🛠 Tools Used

| Tool                          | Purpose                 |
| ----------------------------- | ----------------------- |
| Cisco Packet Tracer           | Network Simulation      |
| Copper Straight-Through Cable | Device Connections      |
| Patch Panel                   | Cable Management        |
| Wall Mount                    | End Device Connectivity |

---

# 🧱 Components Used

| Device      | Quantity |
| ----------- | -------- |
| Patch Panel | 1        |
| Wall Mounts | 2        |
| Switch      | 1        |
| PCs         | 2        |
| Printer     | 1        |
| Server      | 1        |

---

# 📂 Part 1 – Installing the Patch Panel

## Step 1: Open Wiring Closet

* Click the Equipment Cabinet

## Step 2: Add Patch Panel

Navigate to:

```text
Connections → Structured Cabling → Copper Patch Panel
```

Place the patch panel inside the rack.

## Step 3: Rename Patch Panel

Rename the device:

```text
Patch Panel0
```

---

# 🔌 Part 2 – Connecting Switch to Patch Panel

Use Copper Straight-Through cables.

| Switch Port | Patch Panel Port |
| ----------- | ---------------- |
| G1/0/13     | Jack13           |
| G1/0/14     | Jack14           |
| G1/0/15     | Jack15           |
| G1/0/16     | Jack16           |
| G1/0/21     | Jack21           |
| G1/0/22     | Jack22           |
| G1/0/23     | Jack23           |
| G1/0/24     | Jack24           |

---

# 🧱 Part 3 – Adding Wall Mount0

## Install Wall Mount

Navigate to:

```text
Connections → Structured Cabling → Copper Wall Mount
```

Place near the Equipment Cabinet.

Rename it:

```text
Wall Mount0
```

---

# 🔗 Connect Wall Mount0 to Patch Panel

| Wall Mount0 | Patch Panel0 |
| ----------- | ------------ |
| Punchdown1  | Punchdown13  |
| Punchdown2  | Punchdown14  |
| Punchdown3  | Punchdown15  |
| Punchdown4  | Punchdown16  |

---

# 💻 Connect End Devices

Connect using Copper Straight-Through cables:

* Office-Admin PC → Wall Mount0
* Printer0 → Wall Mount0

---

# 🌐 DHCP and Connectivity Test

After waiting for DHCP assignment:

1. Open Office-Admin PC
2. Navigate to:

```text
Desktop → Web Browser
```

3. Enter:

```text
office.srv
```

If the page loads successfully, the network is functioning correctly.

---

# 🧱 Part 4 – Adding Wall Mount1

Install another wall mount near the window.

Rename:

```text
Wall Mount1
```

---

# 🔗 Connect Wall Mount1 to Patch Panel

| Wall Mount1 | Patch Panel0 |
| ----------- | ------------ |
| Punchdown1  | Punchdown21  |
| Punchdown2  | Punchdown22  |
| Punchdown3  | Punchdown23  |
| Punchdown4  | Punchdown24  |

---

# 💻 Connect Office-User PC

Connect:

```text
Office-User PC → Wall Mount1
```

using Copper Straight-Through cable.

---

# 🧪 Verification

Verify:

* DHCP IP Assignment
* Browser Connectivity
* Successful Access to:

```text
office.srv
```

---

# ⚠️ Common Mistakes

## ❌ Mixing Jack and Punchdown Ports

### Correct Usage

| Purpose                | Use             |
| ---------------------- | --------------- |
| Switch Connections     | Jack Ports      |
| Wall Mount Connections | Punchdown Ports |

---

## ❌ Wrong Example

```text
Punchdown1 → Jack13
```

---

## ✅ Correct Example

```text
Punchdown1 → Punchdown13
```

---

# 🧠 Key Learning Outcomes

* Understanding enterprise structured cabling
* Learning patch panel architecture
* Real-world office networking simulation
* DHCP-based IP allocation
* Physical network design principles

---

# 📸 Suggested Screenshots for GitHub

Add screenshots of:

* Final topology
* Wiring closet
* Patch panel connections
* Wall mounts
* Successful browser test
* Activity completion score

---

# 🚀 Future Improvements

* Add VLAN configuration
* Add Router for Internet simulation
* Implement Network Security
* Configure Access Control Lists
* Add Wireless Devices

---

# ✅ Final Result

Successfully created a realistic structured cabling infrastructure using Cisco Packet Tracer with:

* Proper Patch Panel Configuration
* Dual Wall Mount Setup
* Functional DHCP Networking
* Successful Web Connectivity

---

# 👨‍💻 Author

Balamutugan
B.Tech Computer Science and Engineering (Cybersecurity Enthusiast)


