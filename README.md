# 🛡️ SOC Analyst Homelab  

Hands-on SOC Analyst homelab simulating brute-force attacks and detection workflows with Splunk, Sysmon, Hydra, and MITRE ATT&CK. Built to practice **threat detection, log analysis, and incident response** in a realistic environment that mirrors enterprise SOC operations.  

![Lab Screenshot](https://github.com/user-attachments/assets/c33e5627-4bb4-4dbe-b789-de9e759fdf8c)  

---

## 🌐 Lab Overview  

**Virtual Machines:**  
- **Kali Linux (Attacker):** Launches brute-force attacks with Hydra  
- **Windows 10 (Victim):** RDP-enabled endpoint with Sysmon logging  
- **Ubuntu Linux (SIEM):** Hosts Splunk Enterprise for log ingestion and analysis  

**Security Tools:**  
- **Hydra:** Executes RDP brute-force attacks  
- **Sysmon:** Provides detailed Windows telemetry  
- **Splunk:** Aggregates logs, detects brute-force attempts, triggers alerts  
- **MITRE ATT&CK:** Maps adversary behavior for structured detection coverage  

---

## 🔎 Detection Scenario  

**Attack Simulated:**  
- RDP brute-force attack launched via Hydra  

**Detection Method:**  
- **Sysmon Logs:** Captured failed authentication attempts  
- **Splunk Search Query:** Correlated repeated logon failures from the same IP  
- **Custom Splunk Alert:** Triggered on brute-force patterns based on frequency and thresholds  

---

## ✅ Results  

- Brute-force detection time reduced to **<30 seconds** with Splunk correlation searches  
- SOC-style pipeline built: Sysmon → Splunk → Automated Alert  
- Incident aligned with **MITRE ATT&CK T1110 (Brute Force)**  
- Documented investigation workflow for SOC-style reporting  

---

## 📸 Screenshots  

- Hydra console running the attack  
- Splunk dashboards/alerts for brute-force detection  
- Windows Event Viewer showing failed logins  
- MITRE ATT&CK reference mapping  

<img width="1205" height="1193" alt="Screenshot 2025-07-20 181443" src="https://github.com/user-attachments/assets/42e3384b-6005-43ee-a3c7-d88abda1ac12" />  
<img width="1262" height="1357" alt="Screenshot 2025-07-20 205152" src="https://github.com/user-attachments/assets/563a0808-01a3-4c01-a7fb-6eca29a5f6ba" />  
<img width="585" height="704" alt="Screenshot 2025-07-20 194553" src="https://github.com/user-attachments/assets/0ac631dc-e7db-43ac-8be1-7b9b363b099a" />  

---

## 💡 Why This Lab?  

This project demonstrates my ability to:  
- Engineer detections in a SIEM (Splunk)  
- Perform threat hunting and alert triage  
- Map attacker behavior to frameworks (MITRE ATT&CK)  
- Document incidents in SOC-style reports  

---

## 🚀 Future Enhancements  

- Add Wazuh or Security Onion for expanded host/network detection  
- Simulate phishing and credential harvesting scenarios  
- Integrate MITRE ATT&CK Navigator for visual coverage mapping  

---

## 📫 Contact  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/chrisbebawy/)  
[![Credly](https://img.shields.io/badge/Credly-Certifications-orange?style=flat&logo=credly)](https://www.credly.com/users/chris-bebawy)  
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?style=flat&logo=github)](https://github.com/MrPeanutButters)  
