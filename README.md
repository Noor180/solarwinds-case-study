# SolarWinds Cyberattack Case Study

This repository contains a detailed case study of the SolarWinds cyberattack — one of the most significant cyber-espionage campaigns in history. The attack is analyzed using the TTP framework (Tactics, Techniques, and Procedures) and assessed for its impact on the CIA Triad (Confidentiality, Integrity, Availability).

---

## 📌 Summary

The SolarWinds cyberattack was a sophisticated supply chain attack that occurred in 2020. Threat actors compromised the Orion software update system of SolarWinds, allowing them to silently infiltrate networks of government agencies and private companies.

---

## 📅 Timeline (Short)

- **March 2020 – June 2020:** Attackers inserted malware into SolarWinds Orion updates.
- **December 2020:** The attack was discovered and publicly disclosed.
- **2021 Onwards:** Investigation, attribution to APT29 (Cozy Bear), and remediation efforts.

---

## ⚙️ Attack Equation

**Attack = Motive + Method + Vulnerability**

- **Motive:** Cyber-espionage (data theft, intelligence gathering)
- **Method:** Supply chain attack through trojanized software updates
- **Vulnerability:** Lack of detection mechanisms and trust in automatic updates

---

## 🎯 TTP Analysis (MITRE ATT&CK)

### Tactics

- **Initial Access:** Supply Chain Compromise
- **Execution:** Malicious DLL execution
- **Persistence:** Scheduled Tasks, Registry Modifications
- **Defense Evasion:** Code Signing, Obfuscated Files
- **Command and Control:** Encrypted communication with external C2 servers
- **Exfiltration:** Data sent to attacker-controlled infrastructure

### Techniques (Selected IDs)

- **T1195.002**: Supply Chain Compromise: Software Update
- **T1059**: Command and Scripting Interpreter
- **T1055**: Process Injection
- **T1071.001**: Web Protocols (HTTPS C2)
- **T1027**: Obfuscated Files or Information

### Purpose

- Gain long-term access to sensitive government and enterprise networks
- Steal confidential data for geopolitical advantage
- Avoid detection using stealthy, well-engineered malware

---

## 🔐 Impact on CIA Triad

| CIA Element      | Impacted? | Description                                                                 |
|------------------|-----------|-----------------------------------------------------------------------------|
| **Confidentiality** | ✅ Yes    | Sensitive data was accessed by unauthorized actors                         |
| **Integrity**       | ✅ Yes    | Trusted software updates were manipulated, impacting system trust          |
| **Availability**    | ❌ No     | The attack did not aim to disrupt or disable services                      |

---

## 👥 Affected Organizations

- U.S. Treasury Department
- Department of Homeland Security
- Microsoft
- FireEye
- More than 18,000 SolarWinds customers (only a small fraction were specifically targeted)

---

## 📄 Contents

- `SolarWinds Supply Chain Attack.docx` — Full written report


## 📚 References

- FireEye Initial Analysis  
- US-CERT Emergency Directive 21-01  
- Microsoft Threat Intelligence Center Reports  
- MITRE ATT&CK Framework

