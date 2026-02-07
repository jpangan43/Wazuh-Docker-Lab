# Wazuh SIEM Architecture

This lab uses a three-tier SIEM architecture:

## Wazuh Manager
- Collects logs from agents
- Performs rule-based analysis
- Generates security alerts

## Wazuh Indexer
- Stores alerts and events
- Enables fast search and correlation

## Wazuh Dashboard
- Visualizes alerts
- Used by SOC analysts for investigation
