
# 🖧 Packet Tracer – Create Realistic Structured Cabling in the Physical Workspace and Cabling Devices in a Rack

![Cisco](https://img.shields.io/badge/Cisco-PacketTracer-blue)
![Networking](https://img.shields.io/badge/Networking-Structured%20Cabling-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📌 Project Overview

This project demonstrates how to build a realistic enterprise structured cabling environment using Cisco Packet Tracer.

The lab simulates a real office infrastructure where:

- Network devices are connected using structured cabling
- Patch panels are installed inside a wiring closet
- Wall mounts are used for office connectivity
- PCs and printers receive automatic IP addresses through DHCP
- End devices communicate with the office server

This project provides hands-on experience in physical networking, cable organization, and enterprise network deployment.

---

# 🎯 Objectives

The main objectives of this project are:

- Install and configure a Patch Panel
- Create structured cabling inside a wiring closet
- Add and configure Wall Mounts
- Connect network devices using Copper Straight-Through cables
- Understand Jack Ports and Punchdown Ports
- Simulate realistic office network infrastructure
- Test connectivity using DHCP and Web Browser access

---

# 🧠 Understanding Structured Cabling

Structured cabling is a standardized way of organizing and managing network cables in offices and enterprise environments.

Instead of directly connecting PCs to switches, enterprise networks use:

```text id="yoky9t"
PC → Wall Mount → Patch Panel → Switch → Server
````

This improves:

* Cable organization
* Maintenance
* Scalability
* Troubleshooting
* Network reliability

---

# 🛠 Software Used

| Software                 | Purpose                     |
| ------------------------ | --------------------------- |
| Cisco Packet Tracer      | Network Simulation          |
| Structured Cabling Tools | Physical Cabling Simulation |

---

# 🧱 Devices and Components Used

| Device                     | Quantity |
| -------------------------- | -------- |
| Office Switch (Office-SW1) | 1        |
| Patch Panel                | 1        |
| Wall Mounts                | 2        |
| PCs                        | 2        |
| Printer                    | 1        |
| Server                     | 1        |

---

# 🖼 Network Architecture

```text id="pjjm7j"
                 ┌─────────────┐
                 │ Office-User │
                 └──────┬──────┘
                        │
                  Wall Mount1
                        │
                        │
┌─────────────┐   Patch Panel0   ┌─────────────┐
│ Office-Admin│───────┬──────────│  Printer0   │
└──────┬──────┘       │          └─────────────┘
       │              │
  Wall Mount0         │
                      │
                Office-SW1
                      │
                Office Server
```

---

# 📂 Project Workflow

The project is divided into 3 major parts:

| Part   | Description                             |
| ------ | --------------------------------------- |
| Part 1 | Install Patch Panel                     |
| Part 2 | Install Wall Mount0 and connect devices |
| Part 3 | Add Wall Mount1 and additional devices  |

---

# 🧩 Part 1 – Installing the Patch Panel

## Step 1 – Open the Wiring Closet

Click:

```text id="gm69hn"
Equipment Cabinet
```

This opens the simulated wiring closet.

---

## Step 2 – Add Patch Panel

Navigate to:

```text id="ggr0hp"
Connections → Structured Cabling → Copper Patch Panel
```

Place the Patch Panel inside the rack.

---

## Step 3 – Rename the Patch Panel

Rename the device exactly as:

```text id="wpdg55"
Patch Panel0
```

⚠️ Important for grading.

---

# 🔌 Part 2 – Connecting Switch to Patch Panel

Use:

```text id="6v1mvr"
Copper Straight-Through Cable
```

---

## Switch to Patch Panel Connections

| Office-SW1 Port | Patch Panel0 Port |
| --------------- | ----------------- |
| G1/0/13         | Jack13            |
| G1/0/14         | Jack14            |
| G1/0/15         | Jack15            |
| G1/0/16         | Jack16            |

---

# 🧱 Part 3 – Installing Wall Mount0

## Step 1 – Add Wall Mount

Navigate to:

```text id="r93avk"
Connections → Structured Cabling → Copper Wall Mount
```

Place the wall mount next to the Equipment Cabinet.

Rename it:

```text id="yjnkhm"
Wall Mount0
```

---

# 🔗 Connecting Wall Mount0 to Patch Panel0

| Wall Mount0 | Patch Panel0 |
| ----------- | ------------ |
| Punchdown1  | Punchdown13  |
| Punchdown2  | Punchdown14  |
| Punchdown3  | Punchdown15  |
| Punchdown4  | Punchdown16  |

---

# 💻 Connecting End Devices

Use Copper Straight-Through cables to connect:

| Device          | Connect To  |
| --------------- | ----------- |
| Office-Admin PC | Wall Mount0 |
| Printer0        | Wall Mount0 |

---

# 🌐 DHCP and Connectivity Verification

After connecting devices:

1. Wait 30–60 seconds
2. Devices receive IP automatically through DHCP

---

## Testing Connectivity

Open:

```text id="5qt0gi"
Office-Admin → Desktop → Web Browser
```

Enter:

```text id="y62c0v"
office.srv
```

If the page loads successfully, the network is functioning correctly.

---

# 🧱 Part 4 – Installing Wall Mount1

Add another wall mount near the window.

Rename it:

```text id="z1d97o"
Wall Mount1
```

---

# 🔗 Connecting Wall Mount1 to Patch Panel0

| Wall Mount1 | Patch Panel0 |
| ----------- | ------------ |
| Punchdown1  | Punchdown21  |
| Punchdown2  | Punchdown22  |
| Punchdown3  | Punchdown23  |
| Punchdown4  | Punchdown24  |

---

# 🔌 Additional Switch Connections

| Office-SW1 Port | Patch Panel0 Port |
| --------------- | ----------------- |
| G1/0/21         | Jack21            |
| G1/0/22         | Jack22            |
| G1/0/23         | Jack23            |
| G1/0/24         | Jack24            |

---

# 💻 Connecting Office-User PC

Connect:

```text id="fqkgcy"
Office-User PC → Wall Mount1
```

using Copper Straight-Through cable.

---

# 🧪 Final Verification

Verify:

* DHCP IP Assignment
* Network Connectivity
* Browser Access to:

```text id="cq5f80"
office.srv
```

---

# ⚠️ Common Mistakes and Troubleshooting

## ❌ Mistake 1 – Mixing Jack and Punchdown Ports

### Correct Usage

| Connection Type        | Port Type       |
| ---------------------- | --------------- |
| Switch Connections     | Jack Ports      |
| Wall Mount Connections | Punchdown Ports |

---

## ❌ Wrong Example

```text id="m2uxm6"
Punchdown1 → Jack13
```

---

## ✅ Correct Example

```text id="0ql4eu"
Punchdown1 → Punchdown13
```

---

# ❌ Mistake 2 – Wrong Cable Type

Always use:

```text id="pbm5h7"
Copper Straight-Through Cable
```

---

# ❌ Mistake 3 – DHCP Not Working

If devices do not get IP addresses:

1. Open PC
2. Navigate to:

```text id="7a7dn4"
Desktop → IP Configuration
```

3. Click:

```text id="v6p1yy"
DHCP
```

---

# 🧠 Key Learning Outcomes

This project helped in understanding:

* Enterprise structured cabling
* Patch panel deployment
* Wall mount configuration
* Physical network infrastructure
* DHCP networking
* Enterprise cable organization
* Real-world office network architecture

---

# 📸 Recommended GitHub Screenshots

Include screenshots of:

* Final network topology
* Wiring closet
* Patch Panel configuration
* Wall Mount connections
* Successful browser connectivity
* Activity completion score

---

# 🚀 Future Improvements

Possible enhancements include:

* VLAN segmentation
* Router configuration
* Wireless network integration
* Firewall deployment
* Intrusion Detection Systems
* Network monitoring tools
* Access Control Lists (ACLs)

---

# ✅ Final Result

Successfully implemented a realistic structured cabling infrastructure in Cisco Packet Tracer with:

* 1 Patch Panel
* 2 Wall Mounts
* Multiple structured cable connections
* DHCP-based IP allocation
* Successful web connectivity
* Enterprise-style cable organization

---

# 👨‍💻 Author

## Balamutugan

B.Tech Computer Science and Engineering
Cybersecurity & Networking Enthusiast

