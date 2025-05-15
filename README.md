# pfSense DMZ Firewall Project

This project simulates a secure enterprise network environment using **pfSense** and **VMware Workstation**. It demonstrates basic firewall segmentation between a **LAN**, a **DMZ** (Demilitarized Zone), and an **Internet WAN connection**.

---
## 🌐 Network Setup

- **pfSense Firewall**  
  - WAN Interface (Internet/NAT)
  - LAN Interface (Internal Network)
  - DMZ Interface (Web Server Zone)

- **Internal Workstation (Windows 10)**  
  - Connected to LAN
  - Should access Internet and DMZ web server over HTTP

- **Web Server (Ubuntu + Apache2)**  
  - Connected to DMZ
  - Hosts a basic HTTP web server

---

## 🛡️ Firewall Rules Summary
- **LAN to Internet**:
    
    LAN users can browse the web and access the Internet freely.
    
- **LAN to DMZ**:
    
    LAN users can only reach the DMZ web server through **HTTP (port 80)**.
    
    All other types of access (like ping, SSH, or file sharing) are blocked.
    
- DMZ to Internet:
  
  DMZ servers can access the Internet for things like software updates, but only on safe ports like **HTTP/HTTPS**.

- **DMZ to LAN**:

  DMZ servers are **not allowed** to talk to the LAN at all, for security reasons.
  
- **Internet to LAN/DMZ**:

  People from the Internet can't access anything inside the LAN or DMZ, unless specific access is set up.

---

## 📸 Screenshots

---

## 📚 What I Learned

---

## 🔥 Future Improvements
