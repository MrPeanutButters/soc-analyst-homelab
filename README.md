# soc-analyst-homelab
Simulated SOC Analyst environment using Kali Linux, Splunk, Sysmon, and Hydra for log analysis and threat detection
# SOC Analyst Homelab

This project simulates a Security Operations Center (SOC) analyst environment using open-source tools in a virtual lab setting. The goal is to practice threat detection, log analysis, and incident response workflows in a hands-on environment that mirrors real-world SOC operations.

---

## Lab Overview

**Virtual Machines Used:**
- **Kali Linux (Attacker):** Used to launch brute-force attacks using Hydra.
- **Windows 10 (Victim):** Configured with RDP and monitored via Sysmon for system activity.
- **Ubuntu Linux (SIEM):** Hosts Splunk Enterprise for log aggregation and analysis.

**Security Tools:**
- **Hydra:** Performs RDP brute-force attacks against the Windows target.
- **Sysmon:** Provides detailed event logging on the Windows VM.
- **Splunk:** Ingests and analyzes logs to detect brute-force activity.
- **MITRE ATT&CK Framework:** Used to map detected adversary behavior.

---

## Detection Scenario

**Attack Simulated:**  
A dictionary-based brute-force attack via RDP using Hydra.

**Detection Method:**
- **Sysmon Logs:** Captures authentication attempts, failed logins, and lockouts.
- **Splunk Search Query:** Searches for repeated failed logon events from the same IP within a short timeframe.

**Custom Alert:**
An alert was configured in Splunk to trigger when brute-force patterns are detected based on event frequency and thresholds.

---

## Screenshots

A visual demonstration of the environment:
- Hydra console running the attack
- Splunk showing brute-force logs and triggered alert
- Event Viewer on the Windows VM showing failed RDP login attempts
- MITRE ATT&CK page used to map the behavior

---

## Why This Lab?

Setting up a homelab like this has allowed me to:
- Practice detection engineering and threat hunting
- Simulate common attack patterns
- Understand log telemetry across operating systems
- Build familiarity with SIEM tools like Splunk
- Reinforce the value of correlation and alerting logic in SOC workflows

---

## Future Enhancements

- Add Wazuh or Security Onion for more robust host-based detection
- Simulate phishing or credential harvesting scenarios
- Integrate MITRE ATT&CK Navigator to visualize coverage

---

## Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/chrisbebawy) or reach out if you're interested in collaborating or offering feedback!
