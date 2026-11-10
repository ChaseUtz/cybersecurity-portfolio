# Splunk Security Dashboard

## Overview

This project documents the creation of a Splunk dashboard used for monitoring security events within my SOC homelab.

The dashboard provides visibility into Windows event logs, Sysmon telemetry, and endpoint activity collected through Splunk Universal Forwarder.

## Environment

### Log Sources

- Windows 11 Endpoint
- Sysmon
- Splunk Universal Forwarder

### SIEM Platform

- Splunk Enterprise
- Ubuntu Server

## Dashboard Goals

- Monitor endpoint activity
- Visualize event volume
- Detect failed logon attempts
- Observe process creation events
- Support threat hunting activities

## Searches Used

### Events by Host

```spl
index=* | stats count by host
```

### Failed Logons

```spl
index=* EventCode=4625
```

### Successful Logons

```spl
index=* EventCode=4624
```

### Process Creation Events

```spl
index=* EventCode=1
```

## Dashboard Panels

### Events by Host

Displays total event counts from all reporting systems.

### Failed Logons

Monitors Windows Event ID 4625 activity.

### Successful Logons

Tracks successful authentication activity.

### Process Creation Activity

Monitors Sysmon Event ID 1 process creation logs.

## Skills Demonstrated

- SIEM Administration
- SPL Query Development
- Log Analysis
- Security Monitoring
- Threat Hunting
- Dashboard Creation

# Splunk Security Dashboard

## Dashboard Overview

<img src="Splunk%20SOC%20Dashboard.png" width="1000">

## Features

- Centralized log collection
- Windows event monitoring
- pfSense firewall monitoring
- Log source visualization
- Event volume tracking

## Skills Demonstrated

- Splunk Enterprise
- SIEM Administration
- SPL
- Log Analysis
- Security Monitoring