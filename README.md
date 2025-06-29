# 🔐 Setup and Use a Firewall on Windows

## 🎯 Objective
Configure and test basic firewall rules to allow or block traffic using **Windows Defender Firewall**.

---

## 🛠️ Tools Used
- Windows 10/11 built-in **Windows Defender Firewall with Advanced Security**
- No additional tools required

---

## 📌 Task Overview

This project demonstrates how to:
1. Open the firewall configuration tool
2. View current rules
3. Add a rule to block inbound traffic on **port 23 (Telnet)**
4. (Optional) Test the rule
5. Remove the rule to restore original state
6. Document the process and understand how firewall filtering works

---

## 🔧 Steps Performed

### 1️⃣ Open Firewall Configuration
- Open Start Menu → Search for  
  **"Windows Defender Firewall with Advanced Security"**  
- Open the application

---

### 2️⃣ View Current Rules
- Navigate to **Inbound Rules**
- Scroll through the list to view active rules

---

### 3️⃣ Add Inbound Rule to Block Port 23
- Go to **Inbound Rules > New Rule**
- Select **Port** → Click **Next**
- Choose **TCP**, type **23** → Click **Next**
- Select **Block the connection** → Next
- Apply to all profiles → Next
- Name the rule `Block_Telnet` → Finish

---

### 4️⃣ Test the Rule (Telnet not installed)
> **Telnet client was not installed on this system**, so connection testing was skipped.  
> Rule creation was verified via the firewall configuration interface.

*To test manually, Telnet can be enabled via:  
`Control Panel > Programs > Turn Windows features on or off > Telnet Client`*

---

### 5️⃣ Remove the Rule
- In **Inbound Rules**, locate `Block_Telnet`
- Right-click → **Delete**

---

## 📷 Screenshots
- Screenshot of the created `Block_Telnet` rule in **Inbound Rules**
- (Optional) Screenshots of rule creation wizard steps

---

## 📄 Summary: How Firewall Filters Traffic

A **firewall** filters incoming and outgoing traffic based on user-defined rules.  
Each rule can:
- Allow or block **specific ports** (e.g., 23 for Telnet, 80 for HTTP)
- Control **TCP/UDP protocols**
- Apply to **Domain, Private, or Public** profiles

By blocking unused or vulnerable ports (like Telnet), you protect your system from unauthorized access or attacks.

---

## ✅ Deliverables
- `README.md` file (this document)
- Screenshots of the firewall rule setup
