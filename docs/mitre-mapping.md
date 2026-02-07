# MITRE ATT&CK Mapping

This document maps detected security events in the Wazuh SIEM lab to the **MITRE ATT&CK framework**.  
It demonstrates how alerts are classified using real-world adversary tactics and techniques.

This approach reflects standard **SOC analyst investigation workflows**.

## Scenario 1: Multiple Failed Login Attempts

**Description:**  
Multiple failed authentication attempts detected from the same source IP.

**Wazuh Alert Type:**  
Authentication failure / brute-force indication

**MITRE ATT&CK Mapping:**
- **Tactic:** Credential Access
- **Technique:** Brute Force (T1110)

**SOC Analyst Action:**
- Identify source IP
- Check if attempts are internal or external
- Escalate if threshold is exceeded

## Scenario 2: Brute Force Attack (Hydra Simulation)

**Description:**  
A brute-force attack simulated using Hydra against a target system.

**Wazuh Alert Type:**  
Multiple authentication failures in short time window

**MITRE ATT&CK Mapping:**
- **Tactic:** Credential Access
- **Technique:** Brute Force (T1110)

**SOC Analyst Action:**
- Confirm attack pattern
- Correlate with source IP reputation
- Recommend blocking IP and password reset

## Scenario 3: Unauthorized File Modification

**Description:**  
Critical system file modified without authorization.

**Wazuh Alert Type:**  
File Integrity Monitoring (FIM)

**MITRE ATT&CK Mapping:**
- **Tactic:** Defense Evasion
- **Technique:** Modify System Files (T1565.001)

**SOC Analyst Action:**
- Validate file change legitimacy
- Identify user/process responsible
- Escalate if unauthorized
