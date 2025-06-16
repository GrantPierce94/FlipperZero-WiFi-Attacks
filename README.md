# Flipper Zero: WiFi Attacks Project

## Project Scope
The Flipper Zero is an ethical hacking tool with a multitude of “fun” capabilities already built-in, including:

- RFID Scanning (e.g. hotel key cards)
- NFC Reading (e.g. credit cards)
- Sub-GHz signal emulation
- Infrared universal remote control

Many resources for the Flipper are open-source, allowing customization and experimentation.  
This project explored the potential of Flipper Zero to launch two distinct wireless attacks:

- **Evil Portal** (Evil Twin MitM Attack)
- **WiFi Marauder** (Deauth + Sniffing)

---

## Attack Techniques

### Evil Portal (Evil Twin Attack)
An Evil Twin attack involves setting up a rogue WiFi access point that impersonates a legitimate one. Common in high-traffic public areas like:

- Cafés
- Airports
- Libraries

When victims connect, attackers can steal credentials or intercept traffic. These fake portals are:

- Easily deployable
- Highly effective in public networks
- Often used as part of broader MitM attacks

### WiFi Marauder
A combination of **deauthentication attacks** and **packet sniffing** to:

- Force users off real networks
- Capture reconnection data and unencrypted traffic
- Perform MiTM analysis on insecure devices

Targets include:

- Public / open networks
- Outdated or misconfigured routers
- Environments lacking WIDS/WIPS protections

---

## Tools Used

- **Flipper Zero**
- WiFi Devboard Addon
- Kali Linux
- Flipper Apps: Evil Portal & WiFi Marauder
- Open-source wireless tooling

---

## Detection & Defense

### Defender Techniques
- Use WPA3 encryption
- Avoid untrusted networks
- Implement WIDS/WIPS (e.g., LOCH AirShield, Palo Alto)
- Enable Multi-Factor Authentication
- Monitor rogue access point activity

### Attacker Techniques
- Wardriving for network reconnaissance
- Passive sniffing & active deauthentication
- Altering HTML/Captive Portal content
- Ethical Consideration: Conduct only in legal, authorized environments

---

## Project Artifacts

- [Flipping Off The World – Project Slides (PPTX)](./Flipping%20Off%20The%20World.pptx)

---

## Ethical Notice

This project was performed in a controlled and academic setting.  
**Do not replicate** these attacks on unauthorized networks.  
The goal is to **understand, detect, and defend** against real-world cybersecurity threats.

---

## Learning Outcomes

- Understood real-world attack vectors using open-source wireless tools
- Gained hands-on experience with Man-in-the-Middle techniques
- Learned defensive measures and detection methods for WiFi threats
- Strengthened cybersecurity research and presentation skills

---

## License

This repository is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more information.
