# SOC Detection Scenarios

## Scenario 1: Failed Login Attempts
- Log source: Authentication logs
- Detection: Multiple failed login attempts
- Result: Alert generated in Wazuh dashboard

## Scenario 2: Brute Force Attack
- Tool: Hydra
- MITRE ATT&CK: T1110
- Result: High-severity alert

## Scenario 3: File Integrity Monitoring
- Activity: Unauthorized file change
- Detection: Wazuh FIM rule triggered
