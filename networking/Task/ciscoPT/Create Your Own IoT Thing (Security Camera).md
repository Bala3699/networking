# 📡 Packet Tracer - Create Your Own IoT Thing (Security Camera)

## 🎯 Objectives
- Create a custom IoT Thing in Packet Tracer
- Configure it as a Security Camera device
- Connect it to a wireless network
- Save it as a reusable device template

---

# 📘 Part 1: Create Your Own Thing

## 🧩 Step 1: Add a New IoT Device

1. Open the Packet Tracer file.
2. From the **Device Selection Box**, go to **Components → Thing**.
3. Drag and drop the **Thing icon** into the workspace.

---

## 🏷️ Step 2: Change Display Name

1. Click on the newly added Thing.
2. Go to the **Config tab**.
3. Change the **Display Name** to:

```

Security Camera

````

---

## ⚙️ Step 3: Configure Thing Using Thing Editor

1. Open the **Thing Editor tab**.
2. Under **Properties**, set:
   - Component Name:  
     ```
     Security Camera
     ```

3. Enable **Digital Interface**:
   - Select **Digital radio button**
   - Set **Slot Mapping → Slot 1**

---

## 🖼️ Step 3.1: Add Custom Icon (Security Camera Image)

1. Open the instruction file for the activity.
2. Download the provided security camera image.
3. Go back to **Thing Editor → Properties**.
4. Click **New** under image section.
5. Select the downloaded image.
6. Click **Open** to import it.

✅ The device icon is now updated to a Security Camera.

---

## 📶 Step 4: Connect to Wireless Network

1. Open the **I/O Config tab**.
2. Select:
````

Network Adapter → PT-IOT-NM-1W-AC

```
3. Wait for the device to connect.

---

## 🌐 Step 4.1: Verify IP Address

1. Go to **Config tab → Wireless0 interface**
2. Check IP Configuration:
- IPv4 address will be assigned automatically
- Network: `192.168.25.0/24`

---

## 🔍 Step 5: Test Connectivity

1. Open:
```

Tablet → Desktop → Command Prompt

````
2. Run:

```bash
ping <Security_Camera_IP_Address>
````

3. Successful replies confirm connectivity.

---

# 💾 Part 2: Save the New Device

## 📦 Step 1: Save as Device Template

1. Go to:

```
Tools → Custom Device Dialog
```

2. Click **Select**

3. Click on the **Security Camera** in workspace

4. Set:

   * ✔ Home checkbox enabled

5. Click:

```
Add → Save (Template Folder)
```

---

## 📂 Step 2: Verify Saved Template

1. Go to:

```
File → New
```

2. Open Device Selection Box
3. Navigate to **Home section**
4. Confirm:

```
Security Camera is available as a reusable device
```

---

# 🧠 Result

* Created a custom IoT Security Camera
* Configured hardware and network settings
* Connected it to Wi-Fi
* Tested network connectivity
* Saved it as a reusable Packet Tracer template

---

# 🏁 End of Activity



