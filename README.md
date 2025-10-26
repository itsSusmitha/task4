# 🧩 Task 3 - Vulnerability Scan

---

## 🧠 Objective
The objective of this task was to perform a vulnerability scan on the local PC using **Nessus Essentials**, identify common system-level weaknesses, and learn how to interpret and mitigate them effectively.

---

## 🧰 Tools Used
- **Tool:** Nessus Essentials (Free Version)
- **Target:** Localhost (127.0.0.1)
- **Policy:** Basic Network Scan
- **CVSS Version:** v3.0
- **Scan Type:** Local / Credentialed Scan

---

## 🕒 Scan Details
| Parameter | Value |
|------------|--------|
| **Start Time** | 10:29 PM |
| **End Time** | 10:45 PM |
| **Duration** | 17 minutes |
| **Total Vulnerabilities** | 24 |
| **Severity Breakdown** | 3 Critical · 6 High · 8 Medium · 7 Low |

---

## ⚠️ Top 3 Critical Vulnerabilities

### 1. Outdated Software Detected
- **CVSS:** 9.0 (Critical)
- **Description:** The scan detected outdated system or third-party software versions vulnerable to known exploits.
- **Risk Impact:** Could lead to malware infection or privilege escalation.
- **Remediation:** Apply the latest patches via Windows Update or official vendor patches.

### 2. SMB Signing Not Required
- **CVSS:** 8.1 (High)
- **Description:** SMB signing is disabled, which could allow an attacker to intercept SMB traffic.
- **Risk Impact:** Enables man-in-the-middle (MITM) exploitation.
- **Remediation:** Enable SMB signing from Local Group Policy →  
  *Computer Configuration → Windows Settings → Security Options.*

### 3. Open Port 3389 (RDP)
- **CVSS:** 8.4 (High)
- **Description:** RDP port is open, potentially exposing the host to brute-force attacks.
- **Risk Impact:** Allows remote login attempts and compromise risks.
- **Remediation:** Disable RDP if unnecessary or restrict access through a firewall or VPN.

---

## 🧩 Key Learnings
- Gained practical experience using **Nessus Essentials** for vulnerability scanning.
- Learned to interpret and prioritize vulnerabilities based on **CVSS scoring**.
- Understood how misconfigurations and outdated patches increase attack surfaces.
- Learned the importance of consistent patch management and security baselines.

---

## 📸 Screenshots
- `1_summary.png` - Overall Scan Summary  
- `2_vulnerabilities.png` - Vulnerability List  

---

## ✅ Conclusion
This exercise provided hands-on understanding of how vulnerability scanners like **Nessus** help in identifying, ranking, and addressing security weaknesses. It reinforced the importance of applying patches, securing network services, and following security best practices.
