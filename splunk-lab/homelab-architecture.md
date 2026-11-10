# Splunk SOC Homelab Architecture

## Overview

Built a Security Operations Center (SOC) homelab using Hyper-V virtualization, Ubuntu Server, Splunk Enterprise, Sysmon, and Windows 11. The environment was designed to centralize logging, monitor endpoint activity, and support threat hunting and incident investigation exercises.

## Infrastructure

### Hyper-V Host

- Windows 11 Gaming Desktop
- Hyper-V Virtualization Platform

### Splunk Server

- Ubuntu Server
- Splunk Enterprise
- Log Collection and Analysis

### Windows Endpoint

- Windows 11
- Sysmon
- Splunk Universal Forwarder

## Architecture

```text
Windows 11 Endpoint
        │
        ▼
Universal Forwarder
        │
        ▼
Splunk Enterprise (Ubuntu Server)
        │
        ▼
Search, Monitoring, and Investigation
```

## Security Monitoring Goals

- Centralized Logging
- Threat Hunting
- Alert Triage
- Incident Response
- Endpoint Monitoring

## Skills Demonstrated

- SIEM Administration
- Windows Event Analysis
- Sysmon Configuration
- Splunk Search Processing Language (SPL)
- Hyper-V Administration
- Log Analysis
- Security Monitoring

## Future Enhancements

- Add Kali Linux log collection
- Integrate pfSense firewall logs
- Create Splunk security dashboards
- Develop custom detection searches
- Simulate real-world attack scenarios
